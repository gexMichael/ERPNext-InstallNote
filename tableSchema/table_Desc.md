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

