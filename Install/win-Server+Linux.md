在 Windows Server 2012 上架設 Oracle VirtualBox 虛擬機並安裝 Linux，以及將其與 Windows IIS 整合為多站服務，您可以按照以下步驟進行操作：

### 步驟 1：安裝 Oracle VirtualBox
1. **下載 VirtualBox**：從 Oracle 官方網站下載 VirtualBox 的最新版本。
2. **安裝 VirtualBox**：運行安裝程序，按照提示完成安裝過程。選擇適合您需要的安裝目錄和組件。
3. **安裝 VirtualBox Extension Pack**：這個擴展包提供了額外的功能，如 USB 2.0/3.0 支持和 PXE 引導。從 VirtualBox 官方網站下載並安裝該擴展包。

### 步驟 2：建立 Linux 虛擬機 (VM)
1. **啟動 VirtualBox**：打開 VirtualBox 軟件，點擊 "New" 按鈕以創建一個新的虛擬機。
2. **配置虛擬機**：
   - **名稱和操作系統**：輸入虛擬機的名稱（例如 "Linux Server"），選擇 "Linux" 類型和相應的版本（例如 "Ubuntu (64-bit)"）。
   - **內存大小**：分配足夠的內存（建議至少 2GB 或更多）。
   - **硬碟配置**：選擇 "Create a virtual hard disk now"，並選擇 VDI 格式，指定動態分配或固定大小的虛擬磁碟。
3. **安裝 Linux**：
   - **下載 Linux ISO 映像**：從官方網站下載您希望安裝的 Linux 發行版本（例如 Ubuntu、CentOS）。
   - **附加 ISO 文件**：在虛擬機設置中，進入 "Storage" 設置，將下載的 Linux ISO 文件附加為虛擬光碟。
   - **啟動虛擬機**：選擇虛擬機並啟動，然後按照提示安裝 Linux。設置網絡、用戶名和密碼。

### 步驟 3：配置 Linux 和 Windows 網絡
1. **設定網絡類型**：在 VirtualBox 中設置 Linux VM 的網絡為 "Bridged Adapter" 或 "Host-Only Adapter"，使其能夠與 Windows Server 直接通信。
2. **確認網絡連接**：在 Linux 中配置靜態 IP 地址，並確保其與 Windows Server 在同一網段內，以便能相互通信。

要在 Windows Server 2012 的 IIS 中使用 URL Rewrite 將請求轉發到配置了靜態 IP 地址 `192.168.1.196` 的 Linux 虛擬機（VM）上的網站，您可以按照以下步驟進行設置。這樣的配置將實現反向代理，使特定 URL 路徑的請求被重寫並轉發到內部網絡的 Linux 服務器。

### 步驟 4：安裝 URL Rewrite 模塊和 Application Request Routing (ARR)
1. **下載並安裝 URL Rewrite 模塊**：
   - 轉到 [Microsoft 官方網站](https://www.iis.net/downloads/microsoft/url-rewrite)下載並安裝 URL Rewrite 模塊。

2. **下載並安裝 Application Request Routing (ARR)**：
   - 從 [IIS 官方網站](https://www.iis.net/downloads/microsoft/application-request-routing)下載並安裝 Application Request Routing 模塊。

   安裝 ARR 是必要的，因為它提供反向代理功能。

### 步驟 5：啟用反向代理功能
1. **啟用反向代理**：
   - 打開 **IIS 管理器**。
   - 點擊主機名（服務器級別）以進行全局配置。
   - 在 **功能視圖** 中，找到並雙擊 **Application Request Routing Cache**。
   - 在右側操作面板中，點擊 **Server Proxy Settings**。
   - 勾選 **Enable proxy**，然後點擊 **Apply**。

![image](https://github.com/user-attachments/assets/7a36244d-70a6-489e-9bce-5266c8578bdb)

![image](https://github.com/user-attachments/assets/9e340487-aece-4920-be2f-4636f5a2a185)

### 步驟 6：創建 URL Rewrite 規則
1. **選擇目標站點**：
   - 在 **IIS 管理器**中，展開 **Sites** 節點，選擇您要為其設置 URL Rewrite 的目標站點。

2. **打開 URL Rewrite 模塊**：
   - 在選中的網站下，找到並雙擊 **URL Rewrite**。

3. **新增規則**：
   - 在右側的操作面板中，點擊 **Add Rule(s)…**。
   - 選擇 **Blank rule**（空白規則），然後點擊 **OK**。

4. **配置 URL Rewrite 規則**：
   - 為新規則命名，例如 `Reverse Proxy to Linux VM`。
   - **匹配 URL** 部分設置：
     - **Requested URL**：選擇 **Matches the Pattern**。
     - **Using**：選擇 **Regular Expressions**。
     - **Pattern**：輸入 `.*`（表示所有 URL）。
   - **條件**部分：
     - 如果需要僅針對特定路徑設置反向代理，可以點擊 **Add** 以新增條件，例如：`{HTTP_HOST}` equals `example.com` 或 `{REQUEST_URI}` matches `/path/*`。
   - **動作**部分：
     - **Action type**：選擇 **Rewrite**。
     - **Rewrite URL**：輸入 `http://192.168.1.196/{R:0}`，其中 `192.168.1.196` 是 Linux VM 的 IP 地址。
     - **Append query string**：確保選中。
   - 點擊 **Apply** 保存設置。

### 步驟 7：測試反向代理規則
1. **測試設置**：
   - 使用瀏覽器訪問 IIS 服務器的公共 IP 地址或域名，檢查請求是否被正確轉發到 Linux VM 上的網站（IP 地址 `192.168.1.196`）。
   - 例如，訪問 `http://example.com` 時應該被重寫並指向 `http://192.168.1.196`。

2. **檢查日誌和狀態**：
   - 如果請求無法成功轉發，請檢查 IIS 日誌、URL Rewrite 規則和防火牆設置，確保網絡通信沒有被阻斷。

### 注意事項
- **防火牆設置**：確保 Windows Server 和 Linux VM 之間的網絡通信沒有被防火牆阻擋，特別是端口 80（HTTP）或 443（HTTPS）。
- **SSL 支持**：如果使用 HTTPS，還需要在 IIS 中配置 SSL 並確保 ARR 支持 HTTPS 的反向代理。
- **性能優化**：根據負載和網絡配置調整 ARR 的緩存設置以優化性能。

這樣的設置將允許您在 Windows Server 2012 上運行多個站點，其中部分站點服務來自於安裝在 VirtualBox 虛擬機中的 Linux 服務器。
