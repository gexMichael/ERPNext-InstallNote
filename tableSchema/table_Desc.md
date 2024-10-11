以下是 EN 表格和序列的中文名稱翻譯及簡要說明：

### 資料表名稱

| 資料表名稱                | 中文名稱                  | 說明                                              |
|--------------------------|---------------------------|---------------------------------------------------|
| `__Auth`                 | 驗證資料表                | 儲存與系統使用者驗證相關的資料，如密碼哈希等。    |
| `__UserSettings`         | 使用者設定                | 儲存使用者的個人化設置，例如界面配置、偏好等。    |
| `__global_search`        | 全域搜尋                  | 儲存全域搜尋的索引，以提高系統內部搜尋速度。      |

### 序列名稱

| 序列名稱                        | 中文名稱                    | 說明                                                      |
|--------------------------------|-----------------------------|-----------------------------------------------------------|
| `bisect_nodes_id_seq`          | 分叉節點 ID 序列            | 與系統內部進行二分搜尋演算法的節點 ID 自增序列。          |
| `crm_note_id_seq`              | CRM 註記 ID 序列            | 為 CRM（客戶關係管理）註記生成唯一 ID 的自增序列。        |
| `ledger_health_id_seq`         | 帳簿健康狀況 ID 序列        | 用於記錄與財務帳簿健康狀況相關的資料，自動生成 ID。       |
| `prospect_opportunity_id_seq`  | 潛在機會 ID 序列            | 為潛在商機（例如銷售線索）生成唯一 ID 的自增序列。        |
| `pwa_notification_id_seq`      | PWA 通知 ID 序列            | 用於進行進階網頁應用程式（PWA）通知的自增 ID 序列。       |

### 說明：
- **`__Auth`** 和 **`__UserSettings`** 是系統表格，用於管理使用者的登入資料及其個人化設定。
- **`__global_search`** 是系統表格，用於提高系統內部的搜尋效能。
- 序列（例如 `bisect_nodes_id_seq`）通常用於生成唯一的自增主鍵 ID，以便在不同的功能模組中跟蹤和管理資料。

這些表格和序列主要屬於 ERPNext 的底層基礎設施，直接管理系統的操作。如果有需要這些表格的詳細內容或如何匯出這些表格的資訊，請隨時告訴我！

這些是 ERPNext 中一些常見的資料表名稱。以下是這些資料表的中文名稱對應翻譯及簡要說明：

| 資料表名稱                      | 中文名稱                 | 說明                                         |
|---------------------------------|--------------------------|----------------------------------------------|
| `tabAbout Us Team Member`       | 關於我們團隊成員         | 儲存網站中“關於我們”部分的團隊成員資訊。     |
| `tabAccess Log`                 | 訪問日誌                 | 記錄使用者對系統的訪問活動。                 |
| `tabAccount`                    | 帳戶                     | 會計系統中的帳戶資訊（如資產、負債、收入等）。|
| `tabAccount Closing Balance`    | 帳戶結餘                 | 記錄會計期間內帳戶的結餘資訊。               |
| `tabAccounting Dimension`       | 會計維度                 | 定義額外的會計維度（如部門、項目等）。       |
| `tabAccounting Dimension Detail`| 會計維度明細             | 儲存與特定會計維度相關的詳細資料。           |
| `tabAccounting Dimension Filter`| 會計維度過濾             | 用於過濾特定會計維度的資料。                 |
| `tabAccounting Period`          | 會計期間                 | 定義公司的會計期間，例如年度、季度。         |
| `tabActivity Cost`              | 活動成本                 | 儲存與活動相關的成本資料。                   |
| `tabActivity Log`               | 活動日誌                 | 記錄系統內部或使用者的活動紀錄。             |
| `tabActivity Type`              | 活動類型                 | 定義專案、任務等活動的類型。                 |
| `tabAdditional Salary`          | 額外薪資                 | 記錄員工的額外薪酬，例如獎金、津貼。         |
| `tabAddress`                    | 地址                     | 儲存與客戶、供應商、員工等相關的地址資訊。   |
| `tabAddress Template`           | 地址範本                 | 定義不同地區使用的地址格式範本。             |
| `tabAdvance Tax`                | 預繳稅款                 | 記錄公司預繳的稅款資訊。                     |
| 資料表名稱                           | 中文名稱                     | 說明                                                         |
|--------------------------------------|------------------------------|--------------------------------------------------------------|
| `tabAdvance Taxes and Charges`       | 預繳稅款與費用               | 管理預繳稅款和相關費用的資訊。                               |
| `tabAllowed Dimension`               | 允許的會計維度               | 定義允許使用的會計維度，如部門、項目等。                     |
| `tabAllowed To Transact With`        | 允許交易對象                 | 定義可以進行交易的對象，如特定客戶或供應商。                 |
| `tabAmended Document Naming Settings`| 修訂文件命名設置             | 管理修訂文件的命名規則和設置。                               |
| `tabApplicable On Account`           | 適用於帳戶                   | 定義特定規則或設定適用於哪些帳戶。                           |
| `tabAppointment`                     | 預約                         | 管理預約的資訊，如客戶預約時間和細節。                       |
| `tabAppointment Booking Slots`       | 預約預訂時段                 | 定義預約的可預訂時段。                                       |
| `tabAppointment Letter`              | 預約信函                     | 管理與預約相關的信函或通知。                                 |
| `tabAppointment Letter Template`     | 預約信函範本                 | 定義預約信函的範本和格式。                                   |
| `tabAppointment Letter Content`      | 預約信函內容                 | 儲存預約信函的具體內容。                                      |
| `tabAppraisal`                       | 評估                         | 管理員工或項目的評估資訊。                                   |
| `tabAppraisal Cycle`                 | 評估周期                     | 定義評估的周期和頻率。                                         |
| `tabAppraisal Goal`                  | 評估目標                     | 定義評估過程中的目標和指標。                                 |
| `tabAppraisal KRA`                   | 評估關鍵結果區域（KRA）       | 管理評估中的關鍵結果區域。                                     |
| `tabAppraisal Template`              | 評估範本                     | 定義評估過程的範本和標準。                                   |
| `tabAppraisal Template Goal`         | 評估範本目標                 | 定義評估範本中的具體目標。                                     |
| `tabAppraisee`                       | 被評估人                     | 管理被評估的員工或項目。                                       |
| `tabAsset`                           | 資產                         | 管理公司的資產資訊。                                           |
| `tabAsset Activity`                  | 資產活動                     | 記錄與資產相關的各種活動。                                     |
| `tabAsset Capitalization`            | 資產資本化                   | 管理資產的資本化流程和資訊。                                   |
| `tabAsset Capitalization Asset Item` | 資產資本化資產項目           | 定義資產資本化中的資產項目。                                   |
| `tabAsset Capitalization Service Item`| 資產資本化服務項目           | 定義資產資本化中的服務項目。                                   |
| `tabAsset Capitalization Stock Item` | 資產資本化庫存項目           | 定義資產資本化中的庫存項目。                                   |
| `tabAsset Category`                  | 資產類別                     | 定義資產的分類。                                               |
| `tabAsset Category Account`          | 資產類別帳戶                 | 管理資產類別相關的會計帳戶。                                   |
| `tabAsset Depreciation Schedule`     | 資產折舊計劃                 | 管理資產的折舊計劃和安排。                                     |
| `tabAsset Finance Book`              | 資產財務賬簿                 | 管理與資產相關的財務賬簿資訊。                                 |
| `tabAsset Maintenance`               | 資產維護                     | 管理資產的維護和保養資訊。                                     |
| `tabAsset Maintenance Log`           | 資產維護日誌                 | 記錄資產維護活動的詳細日誌。                                   |
| `tabAsset Maintenance Task`          | 資產維護任務                 | 定義和管理資產維護的具體任務。                                 |
| `tabAsset Maintenance Team`          | 資產維護團隊                 | 管理資產維護所需的團隊和成員。                                 |
| `tabAsset Movement`                  | 資產移動                     | 記錄資產的轉移和移動記錄。                                     |
| `tabAsset Movement Item`             | 資產移動項目                 | 管理資產移動中的具體項目。                                     |
| `tabAsset Repair`                    | 資產維修                     | 管理資產的維修和修復資訊。                                     |
| `tabAsset Repair Consumed Item`      | 資產維修消耗項目             | 記錄資產維修過程中消耗的項目。                                 |
| `tabAsset Shift Allocation`          | 資產輪換分配                 | 管理資產輪換和分配的資訊。                                     |
| `tabAsset Shift Factor`              | 資產輪換因素                 | 定義影響資產輪換的因素。                                       |
| `tabAsset Value Adjustment`          | 資產價值調整                 | 管理資產價值的調整和變動。                                     |
|-------------------------------------|------------------------------|--------------------------------------------------------------|
| `tabAssignment Rule`                | 分配規則                     | 定義自動分配任務或工作的規則。                               |
| `tabAssignment Rule Day`            | 分配規則天數                 | 根據日期設定任務分配規則。                                   |
| `tabAssignment Rule User`           | 分配規則使用者               | 管理與分配規則相關的使用者資訊。                             |
| `tabAttendance`                     | 出勤                         | 管理員工的出勤記錄。                                         |
| `tabAttendance Request`             | 出勤請求                     | 員工的出勤請求記錄和狀態。                                   |
| `tabAuthorization Rule`             | 授權規則                     | 管理與系統或業務流程中的授權規則。                           |
| `tabAuto Email Report`              | 自動郵件報告                 | 設定自動生成和發送的報告郵件。                               |
| `tabAuto Repeat`                    | 自動重複                     | 管理週期性事務的自動重複設定。                               |
| `tabAuto Repeat Day`                | 自動重複天數                 | 根據日期設置的自動重複條件。                                 |
| `tabAvailability Of Slots`          | 可用時段                     | 定義或查詢可用的時間時段。                                   |
|-------------------------------------|------------------------------|--------------------------------------------------------------|
| `tabBOM`                            | 物料清單                     | 管理產品的物料清單（BOM）。                                   |
| `tabBOM Creator`                    | BOM 建立者                   | 記錄物料清單的建立者資訊。                                   |
| `tabBOM Creator Item`               | BOM 建立項目                 | 管理物料清單中所包含的具體項目。                             |
| `tabBOM Explosion Item`             | BOM 爆炸項目                 | 列出 BOM 中的所有項目，包含分層結構。                         |
| `tabBOM Item`                       | BOM 項目                     | 管理物料清單中的具體項目。                                   |
| `tabBOM Operation`                  | BOM 操作                     | 定義與 BOM 相關的操作流程。                                   |
| `tabBOM Scrap Item`                 | BOM 廢料項目                 | 管理 BOM 中的廢料資訊。                                       |
| `tabBOM Update Batch`               | BOM 更新批次                 | 管理 BOM 更新的批次記錄。                                     |
| `tabBOM Update Log`                 | BOM 更新日誌                 | 記錄 BOM 更新的操作日誌。                                     |
| `tabBOM Website Item`               | BOM 網站項目                 | 管理在網站上展示的 BOM 項目。                                 |
| `tabBOM Website Operation`          | BOM 網站操作                 | 管理 BOM 在網站上的操作展示。                                 |
|-------------------------------------|------------------------------|--------------------------------------------------------------|
| `tabBank`                           | 銀行                         | 管理銀行的基本資訊。                                           |
| `tabBank Account`                   | 銀行帳戶                     | 記錄公司或個人的銀行帳戶資訊。                                |
| `tabBank Account Subtype`           | 銀行帳戶子類別               | 定義銀行帳戶的子類別。                                        |
| `tabBank Account Type`              | 銀行帳戶類型                 | 定義銀行帳戶的主要類型。                                        |
| `tabBank Clearance Detail`          | 銀行清算明細                 | 記錄銀行交易的清算明細。                                      |
| `tabBank Guarantee`                 | 銀行擔保                     | 管理與銀行擔保相關的資訊。                                    |
| `tabBank Statement Import`          | 銀行對帳單匯入               | 管理銀行對帳單的匯入功能。                                     |
| `tabBank Transaction`               | 銀行交易                     | 記錄銀行交易的詳細資料。                                       |
| `tabBank Transaction Mapping`       | 銀行交易對應                 | 設置銀行交易與 ERPNext 系統的對應規則。                         |
| `tabBank Transaction Payments`      | 銀行交易付款                 | 管理與銀行交易相關的付款資料。                                 |
| `tabBatch`                          | 批次                         | 管理批次管理中的批次資訊。                                     |
| `tabBin`                            | 儲位                         | 記錄倉庫中的儲位資訊。                                         |
| `tabBisect Nodes`                   | 二分節點                     | 用於二分搜尋演算法的節點記錄。                                 |
| `tabBlanket Order`                  | 大宗訂單                     | 管理與供應商或客戶的長期訂單協議。                             |
| `tabBlanket Order Item`             | 大宗訂單項目                 | 記錄大宗訂單中的具體項目。                                     |
| `tabBlock Module`                   | 模組封鎖                     | 管理和控制系統中某些模組的訪問權限。                           |
|-------------------------------------|-------------------------------|--------------------------------------------------------------|
| `tabBlog Category`                  | 部落格分類                    | 管理部落格文章的分類。                                        |
| `tabBlog Post`                      | 部落格文章                    | 管理部落格的文章內容及發佈資訊。                              |
| `tabBlogger`                        | 部落格作者                    | 管理部落格作者的基本資訊。                                    |
| `tabBraintree Settings`             | Braintree 設定                | 管理與 Braintree 支付網關相關的設置。                         |
| `tabBranch`                         | 分支機構                      | 管理公司或組織的分支機構資訊。                                |
| `tabBrand`                          | 品牌                          | 管理產品或服務的品牌資訊。                                    |
| `tabBudget`                         | 預算                          | 記錄和管理公司的預算計劃。                                    |
| `tabBudget Account`                 | 預算帳戶                      | 管理與預算相關的帳戶資訊。                                    |
| `tabBulk Transaction Log Detail`    | 批量交易日誌詳情              | 記錄批量交易的詳細日誌。                                       |
| `tabCRM Note`                       | CRM 記錄                      | 記錄與客戶管理相關的筆記或交流紀錄。                           |
| `tabCalendar View`                  | 日曆視圖                      | 管理日曆的視圖和排程資訊。                                    |
| `tabCall Log`                       | 通話日誌                      | 記錄客戶或業務夥伴的通話記錄。                                |
| `tabCampaign`                       | 行銷活動                      | 管理行銷活動的詳細資訊。                                       |
| `tabCampaign Email Schedule`        | 行銷活動郵件排程              | 管理行銷活動中電子郵件的發送計劃。                             |
| `tabCampaign Item`                  | 行銷活動項目                  | 記錄行銷活動中的具體項目。                                     |
|-------------------------------------|-------------------------------|--------------------------------------------------------------|
| `tabCashier Closing`                | 出納結算                      | 管理出納結算的操作和日誌。                                     |
| `tabCashier Closing Payments`       | 出納結算付款                  | 記錄出納結算時的付款資訊。                                     |
| `tabChangelog Feed`                 | 更新日誌                      | 管理系統或應用程式的更新日誌。                                 |
| `tabCheque Print Template`          | 支票列印範本                  | 定義支票的列印範本和格式。                                     |
| `tabClient Script`                  | 客戶端腳本                    | 管理和執行在系統前端運行的客戶端腳本。                         |
| `tabClosed Document`                | 關閉文件                      | 記錄已關閉的文件資訊。                                         |
| `tabClosing Stock Balance`          | 結存庫存餘額                  | 管理和記錄期末的庫存餘額。                                     |
| `tabColor`                          | 顏色                          | 定義和管理產品、品牌等的顏色選項。                             |
| `tabComment`                        | 評論                          | 管理系統中與文件相關的評論或回饋。                             |
| `tabCommunication`                  | 通訊記錄                      | 記錄系統中的各種通訊活動，如郵件、消息等。                     |
| `tabCommunication Link`             | 通訊鏈接                      | 管理與通訊相關的鏈接資訊。                                     |
| `tabCommunication Medium`           | 通訊媒介                      | 定義通訊的媒介，如電子郵件、電話等。                           |
| `tabCommunication Medium Timeslot`  | 通訊媒介時段                  | 管理通訊媒介的可用時間段。                                     |
|-------------------------------------|-------------------------------|--------------------------------------------------------------|
| `tabCompany`                        | 公司                          | 管理公司的基本資料和設置。                                     |
| `tabCompany History`                | 公司歷史                      | 記錄公司歷史相關的事件和數據。                                 |
| `tabCompensatory Leave Request`     | 補休請求                      | 管理員工的補休申請流程和狀態。                                 |
| `tabCompetitor`                     | 競爭者                        | 記錄和管理競爭者的資訊。                                       |
| `tabCompetitor Detail`              | 競爭者詳情                    | 詳細記錄競爭者的具體資料和分析。                               |
| `tabConnected App`                  | 已連接應用                    | 管理和記錄與 ERPNext 系統連接的應用程式。                      |
| `tabConsole Log`                    | 控制台日誌                    | 記錄系統控制台的操作日誌。                                     |
| `tabContact`                        | 聯絡人                        | 管理公司或個人聯絡人的詳細資料。                               |
|-------------------------------------|-------------------------------------|--------------------------------------------------------------|
| `tabContact Email`                  | 聯絡人電子郵件                      | 記錄與聯絡人相關的電子郵件地址。                             |
| `tabContact Phone`                  | 聯絡人電話                          | 記錄與聯絡人相關的電話號碼。                                 |
| `tabContract`                       | 合同                                | 管理合同的詳細內容與狀態。                                     |
| `tabContract Fulfilment Checklist`  | 合同履行清單                        | 管理和跟蹤合同的履行檢查表。                                  |
| `tabContract Template`              | 合同範本                            | 定義和管理合同的範本，用於快速生成合同。                      |
| `tabContract Template Fulfilment Terms`| 合同範本履行條款                   | 記錄合同範本中的履行條款。                                    |
| `tabCost Center`                    | 成本中心                            | 管理公司內部的成本中心，用於成本核算和分配。                  |
| `tabCost Center Allocation`         | 成本中心分配                        | 記錄成本在不同成本中心之間的分配情況。                        |
| `tabCost Center Allocation Percentage`| 成本中心分配百分比                 | 設定成本在各成本中心之間的分配比例。                          |
| `tabCountry`                        | 國家                                | 記錄國家或地區的資訊，用於國際業務設定。                      |
| `tabCoupon Code`                    | 優惠券代碼                          | 管理優惠券代碼，用於促銷或折扣活動。                          |
|-------------------------------------|-------------------------------------|--------------------------------------------------------------|
| `tabCurrency`                       | 貨幣                                | 管理系統中的貨幣資訊。                                         |
| `tabCurrency Exchange`              | 貨幣匯率                            | 記錄不同貨幣之間的匯率資訊。                                   |
| `tabCurrency Exchange Settings Details`| 貨幣匯率設置詳情                  | 記錄與貨幣匯率設置相關的詳細資訊。                             |
| `tabCurrency Exchange Settings Result`| 貨幣匯率設置結果                  | 管理貨幣匯率設置的結果數據。                                   |
| `tabCustom DocPerm`                 | 自定義文件權限                     | 設置系統中文件的自定義權限。                                   |
| `tabCustom Field`                   | 自定義欄位                          | 在 ERPNext 中添加自定義欄位以擴展系統功能。                    |
| `tabCustom HTML Block`              | 自定義 HTML 區塊                   | 管理系統中的自定義 HTML 區塊，用於頁面設計。                    |
| `tabCustom Role`                    | 自定義角色                          | 定義和管理系統中的自定義角色，賦予特定權限。                   |
| `tabCustomer`                       | 客戶                                | 記錄公司客戶的基本資料。                                       |
| `tabCustomer Credit Limit`          | 客戶信用額度                        | 管理和設定客戶的信用額度。                                     |
| `tabCustomer Group`                 | 客戶群組                            | 將客戶歸類到不同群組中，以便於管理。                           |
| `tabCustomer Group Item`            | 客戶群組項目                        | 管理屬於特定客戶群組的具體項目。                              |
| `tabCustomer Item`                  | 客戶項目                            | 記錄與客戶相關的具體項目。                                    |
| `tabCustomize Form Field`           | 自定義表單欄位                      | 管理和修改系統表單中的欄位。                                   |
| `tabCustoms Tariff Number`          | 海關稅則號碼                        | 記錄與進出口相關的海關稅則號碼。                               |
| `tabDaily Work Summary`             | 每日工作總結                        | 管理員工每日的工作總結報告。                                   |
| `tabDaily Work Summary Group`       | 每日工作總結群組                    | 管理每日工作總結的群組設定。                                   |
| `tabDaily Work Summary Group User`  | 每日工作總結群組使用者              | 管理屬於特定工作總結群組的使用者。                             |
| `tabDashboard`                      | 儀表板                              | 定義和設置系統中的儀表板，用於展示關鍵數據。                    |
| `tabDashboard Chart`                | 儀表板圖表                          | 在儀表板中顯示的圖表資料。                                     |
| `tabDashboard Chart Field`          | 儀表板圖表欄位                      | 定義儀表板圖表的欄位結構。                                     |
| `tabDashboard Chart Link`           | 儀表板圖表鏈接                      | 定義圖表與其他資料之間的鏈接。                                 |
| `tabDashboard Chart Source`         | 儀表板圖表來源                      | 設定儀表板圖表的數據來源。                                     |
| `tabDashboard Settings`             | 儀表板設定                          | 設置和管理儀表板的整體配置。                                   |
| `tabData Import`                    | 資料匯入                            | 管理系統中的資料匯入功能。                                     |
| `tabData Import Log`                | 資料匯入日誌                        | 記錄資料匯入的操作和日誌。                                     |
| `tabDefaultValue`                   | 預設值                              | 設定系統中的預設值。                                           |
| `tabDeleted Document`               | 刪除文件                            | 記錄已刪除的文件資訊。                                         |
| `tabDelivery Note`                  | 交貨單                              | 管理貨物交付的詳細資料。                                       |
| `tabDelivery Note Item`             | 交貨單項目                          | 記錄交貨單中具體的項目資訊。                                   |
| `tabDelivery Stop`                  | 交貨站點                            | 記錄交貨行程中的站點資訊。                                     |
| `tabDelivery Trip`                  | 交貨行程                            | 管理和記錄交貨的行程資訊。                                     |
| `tabDepartment`                     | 部門                                | 記錄公司的部門結構和部門資訊。                                 |
| `tabDepartment Approver`            | 部門審批者                          | 管理特定部門的審批者設定。                                     |
| `tabDependent Task`                 | 依賴任務                            | 記錄項目或任務中的依賴關係。                                   |
| `tabDepreciation Schedule`          | 折舊計劃                            | 管理資產的折舊計劃和記錄。                                     |
|------------------------------------|-----------------------|--------------------------------------------|
| tabDesignation                     | 職稱                   | 儲存員工的職稱資料。                             |
| tabDesignation Skill               | 職稱技能               | 記錄與職稱相關的技能資訊。                        |
| tabDesktop Icon                    | 桌面圖示               | 儲存桌面應用程序的圖示資訊。                      |
| tabDiscounted Invoice              | 折扣發票               | 記錄提供折扣的發票詳細資料。                       |
| tabDiscussion Reply                | 討論回覆               | 儲存討論話題的回覆資訊。                          |
| tabDiscussion Topic                | 討論主題               | 記錄討論的主題和相關細節。                        |
| tabDocField                       | 文件欄位               | 定義文件的欄位結構和屬性。                        |
| tabDocPerm                        | 文件權限               | 記錄不同用戶對文件的訪問權限。                     |
| tabDocShare                       | 文件共享               | 儲存共享文件的相關資訊。                          |
| tabDocType                        | 文件類型               | 定義系統中的不同文件類型及其屬性。                 |
| tabDocType Action                 | 文件類型操作           | 記錄針對不同文件類型的可用操作。                    |
| tabDocType Layout                 | 文件類型佈局           | 定義文件類型的佈局設置。                           |
| tabDocType Layout Field           | 文件類型佈局欄位       | 定義文件類型佈局中的具體欄位。                     |
| tabDocType Link                   | 文件類型鏈接           | 記錄文件類型之間的關聯。                           |
| tabDocType State                  | 文件類型狀態           | 定義文件類型的狀態和流轉。                         |
| tabDocument Follow                 | 文件跟蹤               | 儲存跟蹤文件變更的紀錄。                           |
| tabDocument Naming Rule            | 文件命名規則           | 定義文件的命名規則和格式。                         |
| tabDocument Naming Rule Condition   | 文件命名規則條件       | 記錄應用於命名規則的具體條件。                     |
| tabDocument Share Key              | 文件共享密鑰           | 儲存文件共享的安全密鑰。                           |
| tabDomain                          | 領域                   | 記錄系統中的域名或網站域。                         |
| tabDowntime Entry                  | 停機記錄               | 記錄系統或服務的停機事件。                          |
| tabDriver                          | 駕駛員                 | 儲存駕駛員的基本資訊。                             |
| tabDriving License Category        | 駕駛執照類別           | 定義不同類型的駕駛執照。                           |
| tabDunning                         | 催款                   | 記錄催款過程和相關資訊。                           |
| tabDunning Letter Text             | 催款信內容             | 儲存催款信的模板內容。                             |
| tabDunning Type                    | 催款類型               | 定義不同類型的催款方式。                           |
| tabDynamic Link                    | 動態鏈接               | 記錄系統中動態生成的鏈接。                          |
| tabEmail Account                   | 郵件帳戶               | 儲存與電子郵件相關的帳戶資訊。                      |
| tabEmail Campaign                  | 郵件活動               | 記錄電子郵件營銷活動的詳細資料。                    |
| tabEmail Digest                    | 郵件摘要               | 儲存定期發送的電子郵件摘要。                        |
| tabEmail Digest Recipient           | 郵件摘要接收者         | 記錄郵件摘要的接收者列表。                         |
| tabEmail Domain                    | 郵件域                 | 定義用於電子郵件的域名設定。                        |
| tabEmail Flag Queue                | 郵件標記佇列           | 記錄需要標記或分類的電子郵件佇列。                  |
| tabEmail Group                     | 郵件群組               | 儲存電子郵件群組的詳細資訊。                        |
| tabEmail Group Member              | 郵件群組成員           | 記錄屬於電子郵件群組的成員資訊。                    |
| tabEmail Queue                     | 郵件佇列               | 儲存待發送的電子郵件佇列。                          |
| tabEmail Queue Recipient            | 郵件佇列接收者         | 記錄電子郵件佇列中的接收者資訊。                    |
| tabEmail Rule                      | 郵件規則               | 定義自動化處理電子郵件的規則。                      |
| tabEmail Template                  | 郵件模板               | 儲存電子郵件的預設模板。                            |
| tabEmail Unsubscribe               | 郵件退訂               | 記錄用戶退訂電子郵件訂閱的資訊。                    |
| tabEmployee                        | 員工                   | 儲存員工的基本資訊和詳細資料。                       |
| tabEmployee Advance                | 員工預支               | 記錄員工的預支金額和相關資訊。                       |
| tabEmployee Benefit Application    | 員工福利申請           | 記錄員工申請福利的詳細資訊。                         |
| tabEmployee Benefit Application Detail | 員工福利申請詳情      | 儲存員工福利申請的具體明細資料。                     |
| tabEmployee Benefit Claim          | 員工福利索賠           | 記錄員工索賠福利的詳細資訊。                         |
| tabEmployee Boarding Activity       | 員工登記活動           | 儲存員工登記過程中的活動記錄。                       |
| tabEmployee Checkin                | 員工簽到               | 記錄員工的簽到信息。                               |
| tabEmployee Cost Center            | 員工成本中心           | 定義與員工相關的成本中心。                           |
| tabEmployee Education              | 員工教育               | 儲存員工的教育背景和學歷資訊。                       |
| tabEmployee External Work History   | 員工外部工作歷史       | 記錄員工在其他公司或組織的工作經歷。                 |
|----------------------------------------|------------------------------|--------------------------------------------|
| tabEmployee Feedback Criteria          | 員工反饋標準                   | 定義員工反饋評估的標準。                          |
| tabEmployee Feedback Rating            | 員工反饋評分                   | 記錄員工反饋的評分資訊。                          |
| tabEmployee Grade                      | 員工等級                       | 儲存員工的等級或級別資訊。                        |
| tabEmployee Grievance                  | 員工申訴                       | 記錄員工提出的申訴和相關處理資訊。                  |
| tabEmployee Group                      | 員工群組                       | 儲存員工的群組分類和管理資訊。                      |
| tabEmployee Group Table                | 員工群組表                    | 記錄群組中員工的詳細資訊。                        |
| tabEmployee Health Insurance           | 員工健康保險                   | 儲存員工的健康保險計劃和相關資訊。                  |
| tabEmployee Incentive                  | 員工獎勵                       | 記錄針對員工的獎勵計劃和詳細資訊。                  |
| tabEmployee Internal Work History      | 員工內部工作歷史               | 儲存員工在公司內部的工作經歷。                      |
| tabEmployee Onboarding                 | 員工入職培訓                   | 記錄員工的入職培訓過程和內容。                      |
| tabEmployee Onboarding Template        | 員工入職培訓模板               | 儲存入職培訓的標準模板和流程。                      |
| tabEmployee Other Income               | 員工其他收入                   | 記錄員工的額外收入來源和詳細資訊。                  |
| tabEmployee Performance Feedback       | 員工績效反饋                   | 儲存對員工績效的評估和反饋記錄。                    |
| tabEmployee Promotion                  | 員工晉升                       | 記錄員工的晉升過程和相關資訊。                      |
| tabEmployee Property History            | 員工財產歷史                   | 儲存員工擁有的財產或資產的歷史記錄。                |
| tabEmployee Referral                   | 員工推薦                       | 記錄員工推薦其他候選人的詳細資訊。                  |
| tabEmployee Separation                  | 員工離職                       | 記錄員工離職的過程和相關資料。                      |
| tabEmployee Separation Template        | 員工離職模板                   | 儲存離職過程的標準模板和步驟。                      |
| tabEmployee Skill                      | 員工技能                       | 記錄員工擁有的技能和專業知識。                      |
| tabEmployee Skill Map                  | 員工技能圖                   | 儲存員工技能的視覺化映射，方便查詢和管理。             |
| tabEmployee Tax Exemption Category     | 員工稅務豁免類別               | 定義員工可申請的稅務豁免類別。                      |
| tabEmployee Tax Exemption Declaration   | 員工稅務豁免申報               | 記錄員工的稅務豁免申報內容。                        |
| tabEmployee Tax Exemption Declaration Category | 員工稅務豁免申報類別 | 記錄不同稅務豁免申報的類別資訊。                    |
| tabEmployee Tax Exemption Proof Submission | 員工稅務豁免證明提交       | 儲存員工提交的稅務豁免證明文件的詳細資訊。           |
| tabEmployee Tax Exemption Proof Submission Detail | 員工稅務豁免證明提交詳情 | 記錄稅務豁免證明提交的具體明細資料。                 |
| tabEmployee Tax Exemption Sub Category  | 員工稅務豁免子類別            | 定義稅務豁免的子類別。                             |
| tabEmployee Training                   | 員工培訓                       | 記錄員工參加的培訓課程和相關信息。                   |
| tabEmployee Transfer                   | 員工調動                       | 記錄員工在公司內部的調動資訊。                       |
| tabEmployment Type                    | 就業類型                       | 定義員工的就業類型（如全職、兼職等）。                 |
| tabEnergy Point Log                   | 能源點記錄                    | 記錄與能源使用相關的點數或數據。                     |
| tabEnergy Point Rule                  | 能源點規則                    | 定義能源點的獲取和使用規則。                         |
| tabError Log                          | 錯誤日誌                       | 記錄系統中發生的錯誤和異常事件。                      |
| tabEvent                              | 活動                           | 儲存公司或組織的活動記錄和相關資訊。                  |
| tabEvent Participants                 | 活動參與者                   | 記錄參加活動的員工或外部參與者的詳細資訊。             |
| tabExchange Rate Revaluation          | 匯率重估                       | 記錄匯率變動的重估資訊。                            |
| tabExchange Rate Revaluation Account   | 匯率重估賬戶                  | 定義與匯率重估相關的賬戶。                           |
| tabExit Interview                     | 離職面談                       | 記錄員工離職時的面談結果和反饋。                      |
| tabExpected Skill Set                 | 預期技能組                    | 定義特定職位所需的技能組合。                          |
| tabExpense Claim                      | 費用申請                       | 記錄員工的費用報銷申請及詳細資料。                   |
| tabExpense Claim Account              | 費用申請賬戶                  | 儲存費用申請中涉及的賬戶資訊。                       |
| tabExpense Claim Advance              | 費用申請預支                  | 記錄員工的費用申請預支金額。                         |
| tabExpense Claim Detail               | 費用申請詳情                  | 儲存費用申請的具體明細資料。                         |
| tabExpense Claim Type                 | 費用申請類型                  | 定義不同類型的費用申請。                            |
| tabExpense Taxes and Charges          | 費用稅金與費用                | 記錄費用申請中涉及的稅金和其他收費資訊。               |
| tabFile                              | 文件                           | 儲存系統中的各種文件和附件。                          |
| tabFinance Book                       | 財務帳本                       | 記錄公司財務交易的帳本。                             |
| tabFiscal Year                        | 財政年度                       | 定義公司的財政年度範圍。                            |
| tabFiscal Year Company                | 財政年度公司                  | 記錄公司在特定財政年度的相關資訊。                    |
| tabForm Tour                         | 表單導覽                     | 定義用戶在使用表單時的導覽流程。                      |
| tabForm Tour Step                    | 表單導覽步驟                  | 記錄表單導覽中的具體步驟和指引。                      |
|--------------------------------------------|------------------------------|--------------------------------------------|
| tabFull and Final Asset                    | 全部及最終資產                | 記錄全數及最終資產的詳細資訊。                      |
| tabFull and Final Outstanding Statement     | 全部及最終未清賬單            | 記錄未清賬單的詳細資訊和結算。                      |
| tabFull and Final Statement                 | 全部及最終報表                | 儲存全數和最終的報表資訊。                          |
| tabGL Entry                                | 總帳條目                      | 記錄總帳中的交易條目。                            |
| tabGender                                  | 性別                          | 定義與員工或客戶相關的性別選項。                    |
| tabGlobal Search DocType                   | 全局搜尋文件類型              | 儲存可進行全局搜尋的文件類型。                      |
| tabGoCardless Mandate                      | GoCardless 授權               | 記錄 GoCardless 的付款授權資訊。                     |
| tabGoCardless Settings                     | GoCardless 設定               | 儲存 GoCardless 的相關設定資訊。                     |
| tabGoal                                    | 目標                          | 記錄公司或部門的目標設定和進度。                     |
| tabGoogle Calendar                         | Google 日曆                  | 儲存與 Google 日曆集成的資訊。                      |
| tabGoogle Contacts                         | Google 聯絡人                | 記錄與 Google 聯絡人集成的資訊。                     |
| tabGratuity                                | 服務費                        | 記錄員工或服務的服務費計算規則。                     |
| tabGratuity Applicable Component           | 服務費適用組件                | 定義可適用於服務費的組件。                           |
| tabGratuity Rule                           | 服務費規則                    | 設定計算服務費的規則。                             |
| tabGratuity Rule Slab                      | 服務費規則區間                | 定義服務費的計算區間和比例。                         |
| tabGrievance Type                          | 申訴類型                      | 記錄員工申訴的類別。                             |
| tabHas Domain                              | 擁有域                        | 記錄用戶或角色擁有的域名資訊。                       |
| tabHas Role                                | 擁有角色                      | 記錄用戶擁有的角色資訊。                             |
| tabHelp Article                            | 幫助文章                      | 儲存用於幫助的文章內容。                             |
| tabHelp Category                           | 幫助類別                      | 定義幫助文章的類別。                             |
| tabHoliday                                  | 假期                          | 記錄公司或部門的假期安排。                          |
| tabHoliday List                            | 假期列表                      | 儲存所有假期的詳細資訊。                           |
| tabHomepage Section                        | 首頁區段                      | 定義首頁上的不同區段和內容。                        |
| tabHomepage Section Card                   | 首頁區段卡片                 | 記錄首頁區段中的卡片內容。                           |
| tabIMAP Folder                             | IMAP 資料夾                  | 記錄與 IMAP 郵件系統相關的資料夾資訊。              |
| tabIdentification Document Type            | 識別文件類型                  | 定義用於身份識別的文件類型。                        |
| tabImport Supplier Invoice                  | 匯入供應商發票                | 記錄供應商發票的匯入過程和詳細資訊。                |
| tabIncome Tax Slab                         | 所得稅檔次                    | 記錄所得稅的不同檔次和稅率。                        |
| tabIncome Tax Slab Other Charges           | 所得稅檔次其他費用           | 記錄所得稅檔次相關的其他費用資訊。                   |
| tabIncoming Call Handling Schedule          | 接聽來電處理排程              | 定義接聽來電的處理流程和時間安排。                  |
| tabIncoming Call Settings                   | 接聽來電設定                 | 記錄與接聽來電相關的設定資訊。                      |
| tabIncoterm                                | 貨物貿易條件                  | 定義貨物運輸和貿易的條件。                          |
| tabIndustry Type                           | 行業類型                      | 記錄不同的行業類型以便分類。                        |
| tabInstallation Note                       | 安裝說明                      | 記錄產品或服務的安裝說明和步驟。                    |
| tabInstallation Note Item                  | 安裝說明項目                  | 儲存安裝過程中的具體項目和要求。                    |
| tabInstalled Application                   | 已安裝應用程序                | 記錄已安裝在系統中的應用程序。                       |
| tabIntegration Request                     | 整合請求                      | 記錄系統間的整合請求和相關資訊。                     |
| tabInterest                                 | 利息                          | 記錄與金融交易或貸款相關的利息資訊。                |
| tabInterview                               | 面試                          | 記錄員工面試的詳細資訊。                           |
| tabInterview Detail                        | 面試詳情                      | 儲存面試過程中的具體詳細資料。                      |
| tabInterview Feedback                      | 面試反饋                      | 記錄對面試過程的反饋和評估。                         |
| tabInterview Round                         | 面試輪次                      | 定義面試的不同輪次及其參與者。                       |
| tabInterview Type                          | 面試類型                      | 記錄不同類型的面試方式。                           |
| tabInterviewer                             | 面試官                        | 儲存參與面試的面試官資訊。                           |
| tabInventory Dimension                     | 庫存維度                      | 定義庫存管理中的維度以便更好地分類和查詢。           |
| tabInvoice Discounting                     | 發票折扣                      | 記錄與發票相關的折扣資訊。                           |
| tabIssue                                   | 問題                          | 記錄系統中發生的問題和異常事件。                      |
| tabIssue Priority                          | 問題優先級                    | 定義問題處理的優先級別。                            |
| tabIssue Type                              | 問題類型                      | 記錄不同類型的問題和報告方式。                       |
| tabItem                                    | 項目                          | 儲存庫存中的商品或服務資訊。                         |
|-------------------------------------------|--------------------------------|---------------------------------------------|
| tabItem Alternative                        | 項目替代品                      | 記錄產品的替代項目資訊。                         |
| tabItem Attribute                          | 項目屬性                        | 定義產品的特定屬性以便分類。                     |
| tabItem Attribute Value                    | 項目屬性值                      | 記錄屬性的具體值和描述。                         |
| tabItem Barcode                           | 項目條碼                        | 儲存項目的條碼資訊以便掃描和識別。               |
| tabItem Customer Detail                    | 項目客戶詳情                    | 記錄特定客戶對產品的詳細資訊。                   |
| tabItem Default                           | 項目預設值                      | 定義產品的預設屬性和設定。                       |
| tabItem Group                             | 項目組別                        | 記錄項目的分類組別以便管理。                     |
| tabItem Manufacturer                       | 項目製造商                      | 記錄產品的製造商資訊。                           |
| tabItem Price                             | 項目價格                        | 記錄產品的定價資訊。                           |
| tabItem Quality Inspection Parameter       | 項目質量檢查參數                | 定義產品質量檢查的具體參數和標準。               |
| tabItem Reorder                           | 項目再訂購                      | 記錄再訂購的規則和最低庫存要求。                 |
| tabItem Supplier                          | 項目供應商                      | 記錄與產品相關的供應商資訊。                     |
| tabItem Tax                               | 項目稅                          | 記錄產品的稅率和相關資訊。                       |
| tabItem Tax Template                       | 項目稅模板                      | 定義應用於產品的稅率模板。                       |
| tabItem Tax Template Detail                | 項目稅模板詳細                  | 記錄稅模板的具體細節和組成部分。                 |
| tabItem Variant                           | 項目變體                        | 記錄同一產品的不同變體資訊。                     |
| tabItem Variant Attribute                  | 項目變體屬性                    | 定義產品變體的特定屬性。                         |
| tabItem Website Specification              | 項目網站規格                    | 記錄在網站上顯示的產品詳細規格。                 |
| tabJob Applicant                           | 職位申請人                      | 記錄申請特定職位的求職者資訊。                   |
| tabJob Applicant Source                    | 職位申請人來源                  | 記錄求職者的來源資訊，例如招聘網站或推薦。       |
| tabJob Card                               | 職位卡片                        | 記錄特定工作任務或項目的詳情。                   |
| tabJob Card Item                          | 職位卡片項目                    | 儲存與工作卡片相關的具體項目資訊。               |
| tabJob Card Operation                      | 職位卡片操作                    | 記錄在工作卡片上執行的具體操作。                 |
| tabJob Card Scheduled Time                 | 職位卡片預定時間                | 記錄工作的預定開始和結束時間。                   |
| tabJob Card Scrap Item                    | 職位卡片報廢項目                | 記錄在工作卡片中報廢的項目。                     |
| tabJob Card Time Log                      | 職位卡片時間記錄                | 記錄與工作卡片相關的時間投入。                   |
| tabJob Offer                              | 職位提供                        | 記錄向求職者提供的職位信息和條件。               |
| tabJob Offer Term                         | 職位提供條款                    | 定義職位提供中的具體條款和條件。                 |
| tabJob Offer Term Template                 | 職位提供條款模板                | 記錄職位提供條款的模板信息。                     |
| tabJob Opening                            | 職位空缺                        | 記錄公司中的職位空缺資訊。                       |
| tabJob Requisition                        | 職位需求                        | 記錄公司對職位的需求和申請資訊。                 |
| tabJournal Entry                          | 日記條目                        | 記錄會計中的日記條目和交易。                     |
| tabJournal Entry Account                   | 日記條目帳戶                    | 儲存與日記條目相關的會計帳戶資訊。               |
| tabJournal Entry Template                  | 日記條目模板                    | 定義用於創建日記條目的模板。                     |
| tabJournal Entry Template Account          | 日記條目模板帳戶                | 記錄日記條目模板中的會計帳戶信息。               |
| tabKRA                                    | 關鍵績效指標                    | 記錄與員工或團隊的關鍵績效指標相關的資訊。       |
| tabKanban Board                           | 看板                              | 記錄和管理項目的看板視圖。                       |
| tabKanban Board Column                    | 看板欄                          | 定義看板中的不同欄位以分類任務。                 |
| tabLDAP Group Mapping                     | LDAP 群組映射                  | 記錄 LDAP 群組與系統用戶的映射關係。              |
| tabLanded Cost Item                       | 落地成本項目                    | 記錄貨物的落地成本明細。                         |
| tabLanded Cost Purchase Receipt           | 落地成本採購收據                | 記錄與落地成本相關的採購收據。                    |
| tabLanded Cost Taxes and Charges          | 落地成本稅費及收費              | 記錄落地成本中包含的稅費及其他收費。               |
| tabLanded Cost Voucher                     | 落地成本憑證                    | 記錄落地成本的會計憑證資訊。                      |
| tabLanguage                                | 語言                          | 記錄系統支持的不同語言選項。                      |
| tabLead                                    | 潛在客戶                        | 記錄潛在客戶的詳細資訊。                          |
| tabLead Source                             | 潛在客戶來源                    | 記錄潛在客戶的來源資訊。                          |
| tabLeave Allocation                        | 假期分配                        | 記錄員工的假期分配資訊。                          |
| tabLeave Application                       | 假期申請                        | 記錄員工提交的假期請求。                          |
| tabLeave Block List                        | 假期阻止列表                    | 定義哪些日期不允許請假。                          |
| tabLeave Block List Allow                  | 假期阻止列表允許                | 記錄允許請假的日期和條件。                        |
|--------------------------------------------|--------------------------------|---------------------------------------------|
| tabLeave Block List Date                   | 假期阻止列表日期                | 記錄在假期阻止列表中不允許請假的具體日期。        |
| tabLeave Encashment                        | 假期現金化                      | 記錄員工假期現金化的請求和處理資訊。             |
| tabLeave Ledger Entry                      | 假期分類帳條目                  | 記錄與假期相關的會計條目和交易。                 |
| tabLeave Period                            | 假期期間                        | 定義員工的假期期間規則和相關設定。               |
| tabLeave Policy                            | 假期政策                        | 記錄公司內部的假期政策和規範。                   |
| tabLeave Policy Assignment                 | 假期政策分配                    | 記錄員工與假期政策的對應關係。                   |
| tabLeave Policy Detail                     | 假期政策詳情                    | 定義假期政策的具體條款和細節。                   |
| tabLeave Type                              | 假期類型                        | 記錄各種假期類型的定義和相關資訊。               |
| tabLedger Health                           | 分類帳健康                      | 記錄會計分類帳的健康狀況和異常監控。             |
| tabLedger Health Monitor Company            | 分類帳健康監控公司              | 記錄需要監控健康狀況的公司資訊。                 |
| tabLedger Merge                            | 分類帳合併                      | 記錄合併多個會計分類帳的操作。                   |
| tabLedger Merge Accounts                    | 分類帳合併帳戶                  | 定義合併時涉及的具體帳戶。                       |
| tabLetter Head                             | 信頭                          | 記錄公司信件的信頭樣式和格式設定。               |
| tabLinked Location                         | 連結位置                        | 記錄與其他位置或系統的連結資訊。                 |
| tabList Filter                             | 列表過濾器                     | 定義在列表視圖中使用的過濾條件。                 |
| tabList View Settings                      | 列表視圖設定                   | 記錄用戶自訂的列表視圖設定和選項。               |
| tabLocation                                 | 位置                          | 記錄公司或業務相關的地理位置資訊。               |
| tabLog Setting User                        | 日誌設定用戶                   | 記錄用戶的日誌設定選項和配置。                   |
| tabLogs To Clear                           | 要清除的日誌                   | 定義需清除的日誌紀錄條目。                       |
| tabLost Reason Detail                      | 遺失原因詳情                    | 記錄物品遺失的原因和具體細節。                   |
| tabLower Deduction Certificate              | 降低扣除證明                    | 記錄與降低扣除相關的證明文件。                   |
| tabLoyalty Point Entry                     | 忠誠度積分條目                  | 記錄顧客的忠誠度積分獲取和使用情況。             |
| tabLoyalty Point Entry Redemption          | 忠誠度積分兌換                  | 記錄顧客兌換忠誠度積分的請求和處理資訊。         |
| tabLoyalty Program                         | 忠誠度計畫                      | 記錄公司推行的忠誠度計畫及其條件。               |
| tabLoyalty Program Collection               | 忠誠度計畫收集                  | 記錄忠誠度計畫收集的相關資訊。                   |
| tabMaintenance Schedule                    | 維護排程                        | 記錄設備或系統的維護排程安排。                   |
| tabMaintenance Schedule Detail              | 維護排程詳情                    | 定義維護排程的具體細節和要求。                   |
| tabMaintenance Schedule Item                | 維護排程項目                    | 記錄維護排程中的具體項目。                       |
| tabMaintenance Team Member                  | 維護團隊成員                    | 記錄參與維護工作的團隊成員資訊。                 |
| tabMaintenance Visit                       | 維護訪問                        | 記錄維護工作訪問的具體資訊。                     |
| tabMaintenance Visit Purpose                | 維護訪問目的                    | 定義維護訪問的具體目的和需求。                   |
| tabManufacturer                             | 製造商                          | 記錄產品的製造商及其相關資訊。                   |
| tabMarket Segment                          | 市場區隔                        | 記錄不同的市場區隔和相關市場策略。               |
| tabMarketing Campaign                      | 行銷活動                        | 記錄公司所推行的行銷活動的詳情。                 |
| tabMaterial Request                        | 物料請求                        | 記錄對物料的請求和需求。                         |
| tabMaterial Request Item                   | 物料請求項目                    | 儲存與物料請求相關的具體項目資訊。               |
| tabMaterial Request Plan Item               | 物料請求計畫項目                | 記錄物料請求的計畫和相關項目。                   |
| tabMilestone                               | 里程碑                          | 記錄項目中的重要里程碑和進展。                   |
| tabMilestone Tracker                       | 里程碑追蹤                      | 用於追蹤項目進度的里程碑工具。                   |
| tabMode of Payment                         | 付款方式                        | 記錄可用的付款方式和選項。                       |
| tabMode of Payment Account                  | 付款方式帳戶                    | 定義與付款方式相關的具體會計帳戶。               |
| tabModule Def                              | 模組定義                        | 記錄系統模組的定義和設定。                       |
| tabModule Onboarding                       | 模組上線                        | 記錄模組上線過程中的相關資訊。                   |
| tabModule Profile                           | 模組配置                        | 定義模組的配置和相關選項。                       |
| tabMonthly Distribution                    | 每月分配                        | 記錄每月的資源或成本分配。                       |
| tabMonthly Distribution Percentage          | 每月分配百分比                  | 記錄每月分配的具體百分比資訊。                   |
| tabMpesa Settings                          | Mpesa 設定                     | 記錄 Mpesa 付款系統的設定和配置。                |
| tabNavbar Item                             | 導航列項目                      | 定義導航列中的各個項目和連結。                   |
| tabNetwork Printer Settings                 | 網路印表機設定                  | 記錄網路印表機的配置和設定選項。                 |
| tabNewsletter                              | 新聞信                          | 記錄公司發送的新聞信的內容和設定。               |
|--------------------------------------------|--------------------------------|---------------------------------------------|
| tabNewsletter Attachment                    | 新聞信附件                      | 記錄與新聞信相關的附件文件。                  |
| tabNewsletter Email Group                   | 新聞信電子郵件群組              | 定義將接收新聞信的電子郵件群組。               |
| tabNon Conformance                          | 不符合項                        | 記錄不符合標準或規範的具體項目。              |
| tabNote                                     | 註解                          | 儲存與特定記錄相關的備註或註解。              |
| tabNote Seen By                             | 註解已讀者                      | 記錄哪些用戶已查看特定註解。                  |
| tabNotification                             | 通知                          | 儲存系統內發送的通知資訊。                    |
| tabNotification Log                         | 通知日誌                      | 記錄所有發送的通知和其狀態。                  |
| tabNotification Recipient                   | 通知接收者                    | 定義接收特定通知的用戶或角色。                |
| tabNotification Settings                    | 通知設定                      | 記錄系統通知的設定選項和偏好。                |
| tabNotification Subscribed Document         | 訂閱的通知文件                 | 記錄用戶訂閱的文件類型和相關通知。            |
| tabNumber Card                              | 號碼卡                        | 記錄分配給特定項目的唯一識別號碼。            |
| tabNumber Card Link                         | 號碼卡連結                    | 定義號碼卡與其他記錄之間的連結。              |
| tabOAuth Authorization Code                  | OAuth 授權碼                  | 記錄用於驗證用戶身份的 OAuth 授權碼。         |
| tabOAuth Bearer Token                        | OAuth 憑證                    | 儲存用於 API 認證的 OAuth 憑證。               |
| tabOAuth Client                             | OAuth 客戶端                   | 記錄已註冊的 OAuth 客戶端資訊。                |
| tabOAuth Client Role                        | OAuth 客戶端角色               | 定義 OAuth 客戶端的角色和權限。                |
| tabOAuth Scope                             | OAuth 範圍                    | 記錄 OAuth 的授權範圍和許可範圍。             |
| tabOffer Term                               | 提供條款                      | 記錄銷售提案中的具體條款和條件。              |
| tabOnboarding Permission                    | 上線許可                      | 定義用戶在上線過程中所需的許可權限。          |
| tabOnboarding Step                          | 上線步驟                      | 記錄上線過程中的具體步驟和流程。              |
| tabOnboarding Step Map                      | 上線步驟映射                  | 定義上線步驟之間的關聯和流向。                |
| tabOpening Invoice Creation Tool Item       | 開放發票創建工具項目           | 記錄開放發票創建過程中的具體項目資訊。        |
| tabOperation                                 | 操作                          | 記錄業務操作的定義和執行。                    |
| tabOpportunity                               | 機會                          | 記錄銷售或業務機會的詳細資訊。                |
| tabOpportunity Item                         | 機會項目                      | 定義與特定機會相關的產品或服務項目。          |
| tabOpportunity Lost Reason                  | 機會失去原因                   | 記錄導致特定機會失敗的原因。                  |
| tabOpportunity Lost Reason Detail           | 機會失去原因詳情               | 提供失去機會原因的具體細節。                  |
| tabOpportunity Type                         | 機會類型                      | 定義不同類型的商業機會。                      |
| tabOverdue Payment                          | 逾期付款                      | 記錄未在截止日期前支付的款項。                |
| tabPOS Closing Entry                        | POS 關閉條目                   | 記錄 POS 系統的日結或關閉操作。               |
| tabPOS Closing Entry Detail                  | POS 關閉條目詳情               | 提供 POS 關閉條目的具體細節。                  |
| tabPOS Closing Entry Taxes                   | POS 關閉條目稅金               | 記錄 POS 關閉條目中的稅金資訊。                |
| tabPOS Customer Group                       | POS 客戶群組                   | 定義在 POS 系統中使用的客戶群組。              |
| tabPOS Field                                | POS 欄位                       | 記錄 POS 系統中的特定欄位和功能。              |
| tabPOS Invoice                              | POS 發票                      | 記錄通過 POS 系統生成的發票資訊。              |
| tabPOS Invoice Item                         | POS 發票項目                   | 定義與 POS 發票相關的具體項目。                |
| tabPOS Invoice Merge Log                     | POS 發票合併日誌               | 記錄發票合併的過程和結果。                     |
| tabPOS Invoice Reference                     | POS 發票參考                   | 定義 POS 發票的參考號碼或標識。                |
| tabPOS Item Group                           | POS 項目群組                   | 記錄 POS 系統中的項目分類群組。                |
| tabPOS Opening Entry                        | POS 開啟條目                   | 記錄 POS 系統的開啟操作或初始化資訊。          |
| tabPOS Opening Entry Detail                   | POS 開啟條目詳情               | 提供 POS 開啟條目的具體細節。                  |
| tabPOS Payment Method                       | POS 付款方式                   | 定義在 POS 系統中可用的付款方式。              |
| tabPOS Profile                              | POS 配置                      | 記錄 POS 系統的配置和設置選項。                |
| tabPOS Profile User                         | POS 配置用戶                   | 定義使用特定 POS 配置的用戶。                  |
| tabPOS Search Fields                        | POS 搜索欄位                   | 記錄在 POS 系統中可用的搜索欄位選項。          |
| tabPSOA Cost Center                         | PSOA 成本中心                   | 記錄特定業務活動的成本中心資訊。               |
| tabPSOA Project                             | PSOA 項目                      | 記錄與 PSOA 相關的項目資訊。                    |
| tabPWA Notification                         | PWA 通知                      | 記錄進行中的 PWA（漸進式網頁應用程式）通知。   |
| tabPackage                                  | 套件                          | 記錄應用程式或功能的打包資訊。                  |
| tabPackage Import                           | 套件匯入                      | 記錄從外部匯入的套件資訊。                      |
|----------------------------------------|----------------------------------|---------------------------------------------|
| tabPackage Release                      | 套件版本                         | 記錄應用程式或功能的版本資訊。                  |
| tabPacked Item                         | 打包項目                         | 記錄已打包的商品或項目資訊。                   |
| tabPacking Slip                        | 包裝單                          | 記錄發貨或包裝的詳細信息，包括項目和數量。     |
| tabPacking Slip Item                   | 包裝單項目                       | 定義包裝單中的具體項目及其數量。                 |
| tabPage                                | 頁面                             | 定義系統中各種頁面的配置和內容。                 |
| tabParty Account                       | 交易方帳戶                       | 記錄與特定交易方相關的帳戶資訊。                |
| tabParty Link                          | 交易方連結                       | 定義交易方之間的關聯或連結。                    |
| tabParty Specific Item                 | 交易方特定項目                   | 記錄特定交易方的獨特項目或服務。                |
| tabParty Type                          | 交易方類型                       | 定義不同類型的交易方，如客戶、供應商等。        |
| tabPatch Log                           | 補丁日誌                         | 記錄應用程式或系統的補丁和更新歷史。            |
| tabPause SLA On Status                 | 狀態下暫停 SLA                   | 定義在特定狀態下暫停服務等級協議（SLA）的規則。  |
| tabPayment Entry                       | 付款條目                         | 記錄付款操作的詳細資訊。                        |
| tabPayment Entry Deduction              | 付款條目扣除                     | 記錄付款條目中的扣除資訊。                      |
| tabPayment Entry Reference               | 付款條目參考                    | 定義與付款條目相關的參考資料。                  |
| tabPayment Gateway                      | 付款網關                         | 記錄用於在線支付的網關資訊。                    |
| tabPayment Gateway Account              | 付款網關帳戶                     | 定義與特定付款網關相關的帳戶資訊。              |
| tabPayment Ledger Entry                 | 付款分類帳條目                   | 記錄付款相關的分類帳條目。                      |
| tabPayment Order                        | 付款訂單                         | 記錄與付款相關的訂單詳細資訊。                  |
| tabPayment Order Reference              | 付款訂單參考                    | 定義與付款訂單相關的參考資料。                  |
| tabPayment Request                      | 付款請求                         | 記錄用戶提交的付款請求的詳細資訊。              |
| tabPayment Schedule                     | 付款計畫                         | 定義付款的計畫和時間表。                        |
| tabPayment Term                        | 付款條件                         | 記錄付款的條件和要求，如到期日等。              |
| tabPayment Terms Template               | 付款條件模板                     | 定義可重用的付款條件模板。                      |
| tabPayment Terms Template Detail        | 付款條件模板詳情                 | 提供付款條件模板中的具體條件和細節。            |
| tabPayroll Employee Detail              | 薪資員工詳細                     | 記錄與特定員工薪資相關的詳細資訊。              |
| tabPayroll Entry                        | 薪資條目                         | 記錄每個薪資週期的薪資計算條目。                |
| tabPayroll Period                       | 薪資期間                         | 定義特定薪資計算的期間。                        |
| tabPayroll Period Date                  | 薪資期間日期                     | 記錄特定薪資期間的開始和結束日期。              |
| tabPeriod Closing Voucher               | 期間結算憑證                     | 記錄會計期間結算的憑證資訊。                    |
| tabPersonal Data Deletion Request       | 個人資料刪除請求                 | 記錄用戶要求刪除其個人資料的請求。              |
| tabPersonal Data Deletion Step          | 個人資料刪除步驟                 | 定義刪除個人資料過程中的具體步驟。              |
| tabPersonal Data Download Request        | 個人資料下載請求                 | 記錄用戶要求下載其個人資料的請求。              |
| tabPick List                            | 拣貨清單                         | 記錄出貨時需要拣選的項目清單。                  |
| tabPick List Item                       | 拣貨清單項目                     | 定義拣貨清單中的具體項目和數量。                |
| tabPlant Floor                          | 生產線                           | 記錄生產或作業的實體位置和配置。                |
| tabPortal Menu Item                     | 門戶菜單項目                     | 定義在用戶門戶上顯示的菜單項目。                |
| tabPortal User                          | 門戶用戶                         | 記錄可以訪問用戶門戶的用戶資訊。                |
| tabPrepared Report                       | 準備報告                         | 記錄生成的報告及其狀態。                        |
| tabPrice List                           | 價格清單                         | 定義商品或服務的價格和條件。                    |
| tabPrice List Country                   | 價格清單國家                     | 記錄與特定國家相關的價格清單。                  |
| tabPricing Rule                         | 定價規則                         | 定義影響商品或服務定價的規則。                  |
| tabPricing Rule Brand                   | 定價規則品牌                     | 記錄與特定品牌相關的定價規則。                  |
| tabPricing Rule Detail                  | 定價規則詳情                     | 提供定價規則中的具體條件和細節。                |
| tabPricing Rule Item Code               | 定價規則項目代碼                 | 記錄與特定項目代碼相關的定價規則。              |
| tabPricing Rule Item Group              | 定價規則項目組                   | 定義影響特定項目組的定價規則。                  |
| tabPrint Format                         | 列印格式                         | 記錄報表或文件的列印格式設定。                  |
| tabPrint Format Field Template          | 列印格式欄位模板                 | 定義在列印格式中使用的欄位模板。                |
| tabPrint Heading                        | 列印標題                         | 定義列印報表的標題和樣式。                      |
| tabPrint Style                          | 列印樣式                         | 記錄列印報表的樣式和設計設定。                  |
| tabProcess Deferred Accounting           | 處理延遲會計                     | 記錄處理延遲的會計項目或交易。                  |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabProcess Payment Reconciliation              | 付款對帳處理                  | 記錄付款對帳的過程和結果。                     |
| tabProcess Payment Reconciliation Log          | 付款對帳處理日誌              | 記錄付款對帳過程中的詳細日誌。                 |
| tabProcess Payment Reconciliation Log Allocations | 付款對帳日誌分配              | 定義與付款對帳日誌中各項分配的關聯。             |
| tabProcess Statement Of Accounts               | 帳戶報表處理                  | 記錄帳戶報表的生成和處理過程。                  |
| tabProcess Statement Of Accounts Customer      | 客戶帳戶報表處理              | 記錄針對特定客戶生成的帳戶報表處理過程。        |
| tabProcess Subscription                         | 訂閱處理                      | 記錄訂閱服務的處理過程。                       |
| tabProduct Bundle                              | 產品組合                      | 定義將多個產品捆綁在一起銷售的組合。             |
| tabProduct Bundle Item                         | 產品組合項目                  | 記錄產品組合中的具體項目及其數量。               |
| tabProduction Plan                             | 生產計畫                      | 定義未來的生產計畫和預測。                      |
| tabProduction Plan Item                        | 生產計畫項目                  | 記錄生產計畫中涉及的具體項目。                   |
| tabProduction Plan Item Reference              | 生產計畫項目參考              | 定義與生產計畫項目相關的參考資料。               |
| tabProduction Plan Material Request            | 生產計畫物料請求              | 記錄根據生產計畫所需的物料請求。                 |
| tabProduction Plan Material Request Warehouse   | 生產計畫物料請求倉庫         | 定義與生產計畫物料請求相關的倉庫信息。           |
| tabProduction Plan Sales Order                 | 生產計畫銷售訂單              | 記錄基於生產計畫生成的銷售訂單。                 |
| tabProduction Plan Sub Assembly Item           | 生產計畫子組裝項目            | 定義生產計畫中的子組裝項目。                     |
| tabProject                                     | 專案                           | 記錄各種專案的詳細資訊，包括進度和狀態。          |
| tabProject Template                            | 專案模板                      | 定義可重用的專案結構和內容模板。                 |
| tabProject Template Task                       | 專案模板任務                  | 記錄專案模板中包含的具體任務。                   |
| tabProject Type                                | 專案類型                      | 定義不同類型的專案，例如內部或外部專案。         |
| tabProject Update                              | 專案更新                      | 記錄專案的最新狀態或變更。                       |
| tabProject User                                | 專案用戶                      | 記錄與專案相關的用戶資訊。                       |
| tabPromotional Scheme                          | 推廣方案                      | 記錄特定的促銷活動或推廣策略。                   |
| tabPromotional Scheme Price Discount           | 推廣方案價格折扣              | 定義推廣方案中適用的價格折扣資訊。               |
| tabPromotional Scheme Product Discount         | 推廣方案產品折扣              | 記錄針對特定產品的促銷折扣資訊。                 |
| tabProperty Setter                             | 屬性設置                      | 定義系統屬性或功能的設置和配置。                 |
| tabProspect                                    | 潛在客戶                      | 記錄可能成為客戶的潛在客戶資訊。                 |
| tabProspect Lead                               | 潛在客戶線索                  | 記錄潛在客戶的詳細線索資訊。                     |
| tabProspect Opportunity                         | 潛在客戶機會                  | 記錄針對潛在客戶的商機資訊。                     |
| tabPurchase Invoice                            | 進貨發票                      | 記錄供應商發出的進貨發票詳情。                   |
| tabPurchase Invoice Advance                    | 進貨發票預付款                | 記錄針對進貨發票的預付款詳情。                   |
| tabPurchase Invoice Item                       | 進貨發票項目                  | 記錄進貨發票中的具體項目及其數量。               |
| tabPurchase Order                              | 採購訂單                      | 記錄向供應商下達的訂單詳情。                     |
| tabPurchase Order Item                         | 採購訂單項目                  | 記錄採購訂單中的具體項目及其數量。               |
| tabPurchase Order Item Supplied                | 採購訂單已供應項目            | 記錄供應商已交付的採購訂單項目。                 |
| tabPurchase Receipt                            | 採購收據                      | 記錄收到的採購收據的詳細資訊。                   |
| tabPurchase Receipt Item                       | 採購收據項目                  | 記錄採購收據中的具體項目及其數量。               |
| tabPurchase Receipt Item Supplied              | 採購收據已供應項目            | 記錄已供應的採購收據項目。                       |
| tabPurchase Taxes and Charges                  | 採購稅費                      | 記錄進貨過程中的稅費和附加費用。                 |
| tabPurchase Taxes and Charges Template         | 採購稅費模板                  | 定義可重用的採購稅費模板。                       |
| tabPurpose of Travel                          | 旅行目的                      | 記錄員工旅行的目的和原因。                       |
| tabPutaway Rule                               | 擺放規則                      | 定義庫存物品的擺放規則和流程。                   |
| tabQuality Action                             | 品質行動                      | 記錄針對品質問題的具體行動或措施。               |
| tabQuality Action Resolution                   | 品質行動解決方案              | 記錄針對品質行動的解決方案和結果。               |
| tabQuality Feedback                            | 品質反饋                      | 記錄用戶對產品或服務的品質反饋。                 |
| tabQuality Feedback Parameter                   | 品質反饋參數                  | 定義用於收集品質反饋的參數和標準。               |
| tabQuality Feedback Template                   | 品質反饋模板                  | 記錄可重用的品質反饋收集模板。                   |
| tabQuality Feedback Template Parameter         | 品質反饋模板參數              | 定義品質反饋模板中使用的參數。                   |
| tabQuality Goal                               | 品質目標                      | 定義應達成的品質目標和標準。                     |
| tabQuality Goal Objective                      | 品質目標對象                  | 記錄達成品質目標所需的具體對象或任務。           |
| tabQuality Inspection                          | 品質檢查                      | 記錄對產品或服務進行的品質檢查的詳細資訊。       |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabQuality Inspection Parameter                 | 品質檢查參數                  | 定義品質檢查中使用的參數和標準。               |
| tabQuality Inspection Parameter Group           | 品質檢查參數組                | 將相關的品質檢查參數分組以便於管理。           |
| tabQuality Inspection Reading                   | 品質檢查讀數                  | 記錄進行品質檢查時獲得的具體讀數或數據。       |
| tabQuality Inspection Template                  | 品質檢查模板                  | 定義可重用的品質檢查流程和參數設定。           |
| tabQuality Meeting                              | 品質會議                      | 記錄與品質相關的會議及其詳細資訊。             |
| tabQuality Meeting Agenda                       | 品質會議議程                  | 定義品質會議的議程內容。                       |
| tabQuality Meeting Minutes                      | 品質會議紀錄                  | 記錄品質會議的討論內容和決策。                 |
| tabQuality Procedure                            | 品質流程                      | 記錄執行品質檢查的具體流程和步驟。             |
| tabQuality Procedure Process                    | 品質流程過程                  | 定義品質檢查過程中的具體執行步驟。             |
| tabQuality Review                               | 品質評估                      | 評估產品或服務的品質標準和表現。               |
| tabQuality Review Objective                     | 品質評估目標                  | 定義品質評估的具體目標和期望。                 |
| tabQuery Parameters                             | 查詢參數                      | 定義在進行數據查詢時使用的參數。               |
| tabQuotation                                    | 報價單                        | 記錄供應商提供的產品或服務的報價資訊。         |
| tabQuotation Item                               | 報價單項目                    | 記錄報價單中具體的產品或服務項目。             |
| tabQuotation Lost Reason                        | 報價單失敗原因                | 記錄報價單未能成功的原因分析。                 |
| tabQuotation Lost Reason Detail                 | 報價單失敗原因詳情            | 針對失敗原因提供的具體詳細資訊。               |
| tabReminder                                     | 提醒                          | 設定各種需要提醒的事項或事件。                 |
| tabReport                                       | 報告                          | 記錄生成的各類報告及其內容。                   |
| tabReport Column                                 | 報告欄位                      | 定義報告中使用的欄位及其內容。                 |
| tabReport Filter                                | 報告篩選器                    | 設定用於篩選報告數據的條件或參數。             |
| tabRepost Accounting Ledger                     | 重新發布會計帳簿              | 記錄會計帳簿的重新發布詳情。                   |
| tabRepost Accounting Ledger Items               | 重新發布會計帳簿項目          | 記錄重新發布會計帳簿中的具體項目。             |
| tabRepost Allowed Types                         | 重新發布允許類型              | 定義可以重新發布的帳簿類型。                   |
| tabRepost Item Valuation                        | 重新發布項目估值              | 記錄重新發布項目的估值資訊。                   |
| tabRepost Payment Ledger                        | 重新發布付款帳簿              | 記錄付款帳簿的重新發布詳情。                   |
| tabRepost Payment Ledger Items                  | 重新發布付款帳簿項目          | 記錄重新發布付款帳簿中的具體項目。             |
| tabRequest for Quotation                        | 請求報價                      | 記錄向供應商請求報價的請求詳情。               |
| tabRequest for Quotation Item                   | 請求報價項目                  | 記錄請求報價中的具體產品或服務項目。           |
| tabRequest for Quotation Supplier               | 請求報價供應商                | 記錄可供應請求報價的供應商資訊。               |
| tabRetention Bonus                              | 留任獎金                      | 記錄對於留任員工的獎金計畫和細則。             |
| tabReview Level                                 | 評審級別                      | 定義評審過程中的不同級別或層級。               |
| tabRole                                        | 角色                          | 定義系統中各種角色及其權限設定。                 |
| tabRole Profile                                 | 角色檔案                      | 記錄角色的具體詳細資訊和權限設定。             |
| tabRoute History                                | 路徑歷史                      | 記錄路徑的變更歷史和相關資訊。                 |
| tabRouting                                      | 路由設定                      | 定義系統中使用的路由配置。                     |
| tabSLA Fulfilled On Status                      | SLA達成狀態                   | 記錄服務級別協議(SLA)的履行狀態。              |
| tabSMS Log                                      | 短信日誌                      | 記錄發送和接收的短信詳情。                     |
| tabSMS Parameter                                 | 短信參數                      | 定義發送短信時使用的參數和設定。               |
| tabSalary Component                             | 薪資組件                      | 記錄薪資計算中的各項組成部分。                 |
| tabSalary Component Account                     | 薪資組件帳戶                  | 記錄與薪資組件相關的會計帳戶。                 |
| tabSalary Detail                                | 薪資詳情                      | 記錄每位員工的具體薪資詳情。                   |
| tabSalary Slip                                  | 薪資單                        | 記錄員工的薪資支付明細。                       |
| tabSalary Slip Leave                            | 薪資單假期                    | 記錄薪資單中假期的詳細資訊。                   |
| tabSalary Slip Loan                             | 薪資單貸款                    | 記錄薪資單中涉及的貸款細節。                   |
| tabSalary Slip Timesheet                        | 薪資單工時記錄                | 記錄薪資單中的工時數據。                       |
| tabSalary Structure                             | 薪資結構                      | 定義公司薪資計算的結構和組成部分。             |
| tabSalary Structure Assignment                  | 薪資結構分配                  | 記錄薪資結構分配給員工的詳細資訊。             |
| tabSales Invoice                                | 銷售發票                      | 記錄客戶的銷售發票詳情。                       |
| tabSales Invoice Advance                        | 銷售發票預付款                | 記錄針對銷售發票的預付款詳情。                 |
| tabSales Invoice Item                           | 銷售發票項目                  | 記錄銷售發票中的具體項目及其數量。             |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabSales Invoice Payment                       | 銷售發票付款                  | 記錄針對銷售發票的付款詳情。                 |
| tabSales Invoice Timesheet                     | 銷售發票工時記錄              | 記錄與銷售發票相關的工時信息。               |
| tabSales Order                                 | 銷售訂單                      | 記錄客戶下的銷售訂單及其詳細資訊。           |
| tabSales Order Item                            | 銷售訂單項目                  | 記錄銷售訂單中的具體產品或服務項目。         |
| tabSales Partner                               | 銷售夥伴                      | 記錄與銷售有關的夥伴或代理商的詳細資訊。     |
| tabSales Partner Item                          | 銷售夥伴項目                  | 記錄銷售夥伴所涉及的具體產品或服務。         |
| tabSales Partner Type                          | 銷售夥伴類型                  | 定義不同類型的銷售夥伴。                     |
| tabSales Person                                | 銷售人員                      | 記錄負責銷售的員工或業務代表的詳細資訊。     |
| tabSales Stage                                 | 銷售階段                      | 定義銷售流程中的不同階段或狀態。             |
| tabSales Taxes and Charges                     | 銷售稅和費用                  | 記錄與銷售相關的稅務和費用信息。             |
| tabSales Taxes and Charges Template            | 銷售稅和費用模板              | 定義常用的銷售稅和費用的模板。               |
| tabSales Team                                  | 銷售團隊                      | 記錄負責特定銷售的團隊成員及其角色。         |
| tabSalutation                                   | 稱謂                          | 定義稱謂，如先生、女士等。                   |
| tabScheduled Job Log                           | 排程作業日誌                  | 記錄系統中排程的作業及其執行狀態。           |
| tabScheduled Job Type                          | 排程作業類型                  | 定義排程作業的不同類型。                     |
| tabSerial No                                   | 序列號                        | 記錄產品或項目的唯一序列號。                 |
| tabSerial and Batch Bundle                     | 序列號和批次組                | 定義包含多個序列號和批次的組合。             |
| tabSerial and Batch Entry                      | 序列號和批次輸入              | 記錄產品的序列號和批次信息。                 |
| tabSeries                                       | 系列                          | 定義用於編號或序列的系列。                   |
| tabServer Script                               | 伺服器腳本                    | 記錄用於自動化和自定義的伺服器端腳本。       |
| tabService Day                                 | 服務天數                      | 記錄服務的時間或天數。                       |
| tabService Level Agreement                      | 服務級別協議                  | 記錄提供的服務水平及相關協議。               |
| tabService Level Priority                       | 服務級別優先級                | 定義服務級別的優先順序。                     |
| tabSession Default                             | 會話預設                      | 記錄用戶會話的預設設定。                     |
| tabSessions                                     | 會話                          | 記錄活動會話的詳細資訊。                     |
| tabShare Balance                               | 股份餘額                      | 記錄股東的股份餘額信息。                     |
| tabShare Transfer                              | 股份轉讓                      | 記錄股份轉讓的詳細資訊。                     |
| tabShare Type                                  | 股份類型                      | 定義不同類型的股份。                         |
| tabShareholder                                 | 股東                          | 記錄公司的股東及其詳細資訊。                 |
| tabShift Assignment                            | 班次分配                      | 記錄員工的班次分配信息。                     |
| tabShift Request                               | 班次請求                      | 記錄員工對班次的請求和變更。                 |
| tabShift Type                                  | 班次類型                      | 定義班次的不同類型。                         |
| tabShipment                                    | 裝運                          | 記錄貨物或產品的裝運詳情。                   |
| tabShipment Delivery Note                      | 裝運交貨單                    | 記錄裝運產品的交貨詳情。                     |
| tabShipment Parcel                             | 裝運包裹                      | 記錄裝運的包裹信息。                         |
| tabShipment Parcel Template                     | 裝運包裹模板                  | 定義包裹的裝運模板。                         |
| tabShipping Rule                               | 裝運規則                      | 定義與裝運相關的規則和條件。                 |
| tabShipping Rule Condition                      | 裝運規則條件                  | 設定裝運規則適用的條件。                     |
| tabShipping Rule Country                        | 裝運規則國家                  | 定義適用於特定國家的裝運規則。               |
| tabSingles                                     | 單身                          | 記錄單身人士的詳細資訊。                     |
| tabSkill                                       | 技能                          | 記錄員工的技能及其相關資訊。                 |
| tabSkill Assessment                             | 技能評估                      | 評估員工技能的過程和結果。                   |
| tabSlack Webhook URL                           | Slack Webhook URL             | 記錄用於與 Slack 集成的 webhook URL。       |
| tabSocial Link Settings                         | 社交鏈接設定                  | 定義用於社交媒體的鏈接設定。                 |
| tabSocial Login Key                             | 社交登入金鑰                  | 記錄社交媒體登入的金鑰設定。                 |
| tabSouth Africa VAT Account                     | 南非增值稅帳戶                | 記錄南非的增值稅帳戶信息。                   |
| tabSouth Africa VAT Settings                    | 南非增值稅設定                | 定義南非增值稅的相關設定。                   |
| tabStaffing Plan                                | 人力資源計畫                  | 記錄公司的人力資源需求計畫。                 |
| tabStaffing Plan Detail                         | 人力資源計畫詳情              | 記錄人力資源計畫的具體詳細資訊。             |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabStock Entry                                  | 存貨輸入                      | 記錄產品進庫的詳細信息。                     |
| tabStock Entry Detail                          | 存貨輸入詳情                  | 記錄每個存貨輸入的具體明細信息。             |
| tabStock Entry Type                           | 存貨輸入類型                  | 定義不同類型的存貨輸入。                     |
| tabStock Ledger Entry                         | 存貨分類帳目                  | 記錄存貨的進出和變動情況。                   |
| tabStock Reconciliation                       | 存貨調整                      | 用於調整存貨數量的過程。                     |
| tabStock Reconciliation Item                  | 存貨調整項目                  | 記錄存貨調整中具體項目的明細。               |
| tabStock Reservation Entry                    | 存貨預留輸入                  | 記錄為了特定訂單而預留的存貨信息。           |
| tabStripe Settings                            | Stripe 設定                  | 記錄與 Stripe 付款網關相關的設定。          |
| tabSub Operation                              | 子操作                        | 定義主操作下的子操作或子任務。               |
| tabSubcontracting BOM                         | 分包物料清單                  | 記錄分包項目的物料需求清單。                 |
| tabSubcontracting Order                       | 分包訂單                      | 記錄分包給供應商的訂單。                     |
| tabSubcontracting Order Item                  | 分包訂單項目                  | 記錄分包訂單中的具體產品或服務項目。         |
| tabSubcontracting Order Service Item          | 分包訂單服務項目              | 記錄分包訂單中的服務項目。                   |
| tabSubcontracting Order Supplied Item         | 分包訂單供應項目              | 記錄從供應商處收到的分包訂單項目。           |
| tabSubcontracting Receipt                     | 分包收據                      | 記錄收到的分包商品的收據。                   |
| tabSubcontracting Receipt Item                | 分包收據項目                  | 記錄分包收據中的具體項目。                   |
| tabSubcontracting Receipt Supplied Item       | 分包收據供應項目              | 記錄分包收據中供應的項目。                   |
| tabSubmission Queue                           | 提交隊列                      | 記錄待處理的提交請求。                       |
| tabSubscription                               | 訂閱                          | 記錄客戶的訂閱服務和計畫。                   |
| tabSubscription Invoice                       | 訂閱發票                      | 記錄針對訂閱服務的發票。                     |
| tabSubscription Plan                          | 訂閱計畫                      | 定義可供選擇的訂閱服務計畫。                 |
| tabSubscription Plan Detail                   | 訂閱計畫詳情                  | 記錄訂閱計畫的具體詳細資訊。                 |
| tabSuccess Action                             | 成功操作                      | 定義成功操作的具體行為或反應。               |
| tabSupplier                                   | 供應商                        | 記錄公司的供應商及其詳細資訊。               |
| tabSupplier Group                             | 供應商群組                    | 記錄供應商的分類或群組信息。                 |
| tabSupplier Group Item                        | 供應商群組項目                | 記錄供應商群組中的具體供應商。               |
| tabSupplier Item                              | 供應商項目                    | 記錄供應商提供的具體產品或服務。             |
| tabSupplier Quotation                         | 供應商報價                    | 記錄供應商的報價信息。                       |
| tabSupplier Quotation Item                    | 供應商報價項目                | 記錄供應商報價中的具體項目。                 |
| tabSupplier Scorecard                         | 供應商評分卡                  | 評估供應商表現的記錄。                       |
| tabSupplier Scorecard Criteria                | 供應商評分標準                | 定義評分供應商的標準。                       |
| tabSupplier Scorecard Period                  | 供應商評分期間                | 記錄評分的期間或時間範圍。                   |
| tabSupplier Scorecard Scoring Criteria        | 供應商評分標準條件            | 記錄用於評分的具體條件。                     |
| tabSupplier Scorecard Scoring Standing        | 供應商評分結果                | 記錄評分結果的詳細信息。                     |
| tabSupplier Scorecard Scoring Variable        | 供應商評分變數                | 記錄影響評分的變數。                         |
| tabSupplier Scorecard Standing                 | 供應商評分地位                | 定義供應商在評分中的地位或排名。             |
| tabSupplier Scorecard Variable                 | 供應商評分變數                | 定義影響評分的特定變數。                     |
| tabSupport Search Source                      | 支持搜索來源                  | 記錄用於搜索支持請求的來源信息。             |
| tabTag                                        | 標籤                          | 記錄用於標記資料的標籤信息。                 |
| tabTag Link                                   | 標籤連結                      | 記錄標籤與其他資料之間的連結。               |
| tabTally Migration                             | Tally 資料遷移                | 記錄從 Tally 系統遷移的資料。                 |
| tabTarget Detail                               | 目標詳情                      | 記錄目標的具體詳細資訊。                     |
| tabTask                                       | 任務                          | 記錄系統中需要完成的任務。                   |
| tabTask Depends On                            | 任務依賴                      | 記錄任務之間的依賴關係。                     |
| tabTask Type                                  | 任務類型                      | 定義任務的不同類型。                         |
| tabTax Category                                | 稅務類別                      | 定義各種稅務的類別或類型。                   |
| tabTax Rule                                   | 稅務規則                      | 記錄適用於稅務的規則。                       |
| tabTax Withheld Vouchers                      | 扣繳憑證                      | 記錄在支付中已被扣繳的稅務憑證。             |
| tabTax Withholding Account                     | 扣繳帳戶                      | 記錄用於扣繳的銀行帳戶信息。                 |
| tabTax Withholding Category                    | 扣繳類別                      | 定義扣繳的不同類別。                         |
| tabTax Withholding Rate                        | 扣繳稅率                      | 記錄適用的扣繳稅率。                         |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabTaxable Salary Slab                        | 可稅薪資檔次                  | 定義不同薪資級別的稅務級別。                   |
| tabTelephony Call Type                        | 電話通話類型                  | 記錄不同類型的電話通話信息。                   |
| tabTerms and Conditions                       | 條款與條件                    | 定義公司服務或產品的使用條款與條件。           |
| tabTerritory                                  | 地區                          | 記錄業務所涉及的地理區域。                     |
| tabTerritory Item                             | 地區項目                      | 記錄特定地區內的產品或服務項目。               |
| tabTimesheet                                  | 工時表                        | 記錄員工的工作時間和項目。                     |
| tabTimesheet Detail                           | 工時表詳情                    | 記錄工時表中的具體詳細項目。                   |
| tabToDo                                       | 待辦事項                      | 記錄需要完成的任務或事項。                     |
| tabToken Cache                                | 令牌快取                      | 用於存儲臨時令牌以提高性能。                   |
| tabTop Bar Item                               | 頂部導航項目                  | 設定應用程式上方導航欄的項目。                 |
| tabTraining Event                             | 培訓事件                      | 記錄進行的培訓活動或事件。                     |
| tabTraining Event Employee                    | 培訓事件員工                  | 記錄參加特定培訓事件的員工信息。               |
| tabTraining Feedback                           | 培訓反饋                      | 記錄參與者對培訓的反饋和評價。                 |
| tabTraining Program                            | 培訓計畫                      | 記錄公司內部的培訓計畫。                       |
| tabTraining Result                             | 培訓結果                      | 記錄員工在培訓計畫中的表現和結果。             |
| tabTraining Result Employee                    | 培訓結果員工                  | 記錄員工在特定培訓中的結果。                   |
| tabTransaction Deletion Record                | 交易刪除記錄                  | 記錄已刪除的交易的詳細信息。                   |
| tabTransaction Deletion Record Details        | 交易刪除記錄詳情              | 記錄已刪除交易的具體細節。                     |
| tabTransaction Deletion Record Item           | 交易刪除記錄項目              | 記錄已刪除交易中的具體項目。                   |
| tabTransaction Log                             | 交易日誌                      | 記錄所有交易的操作日誌。                       |
| tabTranslation                                 | 翻譯                          | 記錄不同語言的文本翻譯。                       |
| tabTravel Itinerary                            | 旅行行程                      | 記錄員工旅行的具體行程安排。                   |
| tabTravel Request                              | 旅行請求                      | 記錄員工提出的旅行請求。                       |
| tabTravel Request Costing                      | 旅行請求成本                  | 記錄旅行請求中的成本預算。                     |
| tabUAE VAT Account                             | 阿聯酋增值稅帳戶              | 記錄阿聯酋的增值稅相關帳戶信息。               |
| tabUAE VAT Settings                            | 阿聯酋增值稅設定              | 記錄阿聯酋增值稅的設定資訊。                   |
| tabUOM                                        | 單位                          | 記錄用於計量的單位。                           |
| tabUOM Category                                | 單位類別                      | 定義不同單位的類別。                           |
| tabUOM Conversion Detail                       | 單位轉換詳情                  | 記錄單位之間的轉換詳細信息。                   |
| tabUOM Conversion Factor                       | 單位轉換因子                  | 定義不同單位之間的轉換比例。                   |
| tabUnhandled Email                             | 未處理的電子郵件              | 記錄尚未處理的電子郵件信息。                   |
| tabUnreconcile Payment                         | 未對賬付款                    | 記錄未對賬的付款交易。                         |
| tabUnreconcile Payment Entries                 | 未對賬付款條目                | 記錄未對賬付款中的具體項目。                   |
| tabUser                                       | 使用者                        | 記錄系統中的用戶信息。                         |
| tabUser Document Type                          | 使用者文件類型                | 定義與用戶相關的文件類型。                     |
| tabUser Email                                  | 使用者電子郵件                | 記錄用戶的電子郵件地址。                       |
| tabUser Group                                  | 使用者群組                    | 記錄用戶的分組信息。                           |
| tabUser Group Member                           | 使用者群組成員                | 記錄特定用戶群組的成員信息。                   |
| tabUser Permission                             | 使用者權限                    | 記錄用戶在系統中的權限設定。                   |
| tabUser Select Document Type                   | 使用者選擇的文件類型          | 記錄用戶可選擇的文件類型。                     |
| tabUser Social Login                           | 使用者社交登錄                | 記錄用戶社交媒體登錄的相關信息。               |
| tabUser Type                                   | 使用者類型                    | 定義用戶的不同類型。                           |
| tabUser Type Module                            | 使用者類型模組                | 定義與用戶類型相關的模組設定。                 |
| tabVariant Field                               | 變體欄位                      | 記錄商品變體的特定屬性或特徵。                 |
| tabVehicle                                     | 車輛                          | 記錄公司的車輛信息。                           |
| tabVehicle Log                                  | 車輛日誌                     | 記錄車輛的使用歷史和維護記錄。                 |
| tabVehicle Service                             | 車輛服務                      | 記錄車輛所需的服務和維護信息。                 |
| tabVehicle Service Item                        | 車輛服務項目                  | 記錄車輛服務中的具體項目。                     |
| tabVersion                                      | 版本                          | 記錄應用程序的版本信息。                       |
|-----------------------------------------------|-------------------------------|---------------------------------------------|
| tabVideo                                       | 視頻                          | 記錄與培訓或行銷相關的視頻文件。               |
| tabView Log                                   | 瀏覽日誌                      | 記錄用戶的瀏覽活動及其行為。                  |
| tabVoice Call Settings                        | 語音通話設置                  | 設定與語音通話相關的參數。                    |
| tabWarehouse                                   | 倉庫                          | 記錄公司倉庫的相關信息。                      |
| tabWarehouse Type                             | 倉庫類型                      | 定義不同類型的倉庫及其屬性。                  |
| tabWarranty Claim                             | 保修索賠                      | 記錄關於產品保修的索賠請求。                  |
| tabWeb Form                                   | 網頁表單                      | 記錄在網站上使用的表單信息。                  |
| tabWeb Form Field                             | 網頁表單欄位                  | 定義網頁表單中的具體欄位。                    |
| tabWeb Form List Column                       | 網頁表單列表欄位              | 記錄在網頁表單列表中顯示的欄位信息。          |
| tabWeb Page                                   | 網頁                          | 記錄網站上的具體網頁信息。                    |
| tabWeb Page Block                             | 網頁區塊                      | 定義網頁中的特定區域或區塊。                  |
| tabWeb Page View                              | 網頁視圖                      | 記錄網頁的顯示和排版設置。                    |
| tabWeb Template                               | 網頁模板                      | 記錄用於生成網頁的模板信息。                  |
| tabWeb Template Field                         | 網頁模板欄位                  | 定義在網頁模板中使用的欄位。                  |
| tabWebhook                                    | 網頁hook                      | 記錄與外部系統集成的webhook設置。            |
| tabWebhook Data                               | 網頁hook數據                  | 記錄與webhook相關的數據。                     |
| tabWebhook Header                             | 網頁hook標頭                  | 定義webhook請求的標頭信息。                   |
| tabWebhook Request Log                        | 網頁hook請求日誌              | 記錄webhook請求的詳細日誌。                   |
| tabWebsite Attribute                           | 網站屬性                      | 定義網站上的屬性和設定。                      |
| tabWebsite Filter Field                       | 網站過濾欄位                  | 設定網站上過濾器的欄位。                      |
| tabWebsite Item Group                         | 網站項目組                    | 定義在網站中使用的產品或項目分組。            |
| tabWebsite Meta Tag                           | 網站元標籤                    | 記錄網站的SEO相關元標籤。                     |
| tabWebsite Route Meta                         | 網站路由元數據                | 定義路由的元數據，以改善網站的導航。          |
| tabWebsite Route Redirect                     | 網站路由重定向                | 設定特定路由的重定向規則。                    |
| tabWebsite Sidebar                            | 網站側邊欄                    | 定義網站側邊欄的內容和配置。                  |
| tabWebsite Sidebar Item                       | 網站側邊欄項目                | 記錄側邊欄中顯示的具體項目。                  |
| tabWebsite Slideshow                          | 網站幻燈片                    | 記錄在網站上使用的幻燈片設置。                |
| tabWebsite Slideshow Item                     | 網站幻燈片項目                | 定義幻燈片中的具體內容項目。                  |
| tabWebsite Theme                              | 網站主題                      | 記錄網站的外觀主題設置。                      |
| tabWebsite Theme Ignore App                   | 網站主題忽略應用              | 設定在使用主題時需要忽略的應用。              |
| tabWork Order                                 | 工作訂單                      | 記錄具體的工作訂單信息。                      |
| tabWork Order Item                            | 工作訂單項目                  | 記錄工作訂單中的具體項目。                    |
| tabWork Order Operation                       | 工作訂單操作                  | 記錄與工作訂單相關的操作記錄。                |
| tabWorkflow                                   | 工作流程                      | 設定業務流程的定義和管理。                    |
| tabWorkflow Action                            | 工作流程動作                  | 記錄在工作流程中可執行的具體動作。            |
| tabWorkflow Action Master                     | 工作流程動作主檔              | 定義可用的工作流程動作的基本設置。            |
| tabWorkflow Action Permitted Role            | 工作流程動作允許角色          | 設定可執行特定工作流程動作的角色。            |
| tabWorkflow Document State                    | 工作流程文件狀態              | 記錄工作流程中文件的當前狀態。                |
| tabWorkflow State                             | 工作流程狀態                  | 記錄工作流程的不同狀態。                      |
| tabWorkflow Transition                        | 工作流程轉換                  | 定義在工作流程中不同狀態之間的轉換規則。      |
| tabWorkspace                                   | 工作區域                      | 記錄用於特定任務的工作區域設定。              |
| tabWorkspace Chart                             | 工作區域圖表                  | 記錄在工作區域中使用的圖表設定。              |
| tabWorkspace Custom Block                     | 工作區域自定義區塊            | 定義在工作區域中使用的自定義區塊。            |
| tabWorkspace Link                              | 工作區域鏈接                  | 記錄工作區域中的鏈接信息。                    |
| tabWorkspace Number Card                       | 工作區域數字卡                | 記錄在工作區域中顯示的數字卡設定。            |
| tabWorkspace Quick List                        | 工作區域快速列表              | 定義在工作區域中顯示的快速訪問列表。          |
| tabWorkspace Shortcut                          | 工作區域快捷方式              | 記錄在工作區域中使用的快捷方式。              |
| tabWorkstation                                 | 工作站                        | 記錄工作站的配置和使用情況。                  |
| tabWorkstation Type                            | 工作站類型                    | 定義不同類型的工作站。                        |
| tabWorkstation Working Hour                    | 工作站工作時間                | 記錄工作站的開放和使用時間。                   |
| web_form_list_column_id_seq                   | 網頁表單列表欄位ID序列        | 記錄用於生成網頁表單列表欄位的自增ID序列。    |



