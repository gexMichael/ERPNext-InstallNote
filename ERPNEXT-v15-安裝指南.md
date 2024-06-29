**安裝環境：Ubuntu Server 22.04 Lts** 

1. 如果當前登錄的是root用戶，就請新建一個用於安裝ERP的sudo用戶。如果已經有sudo組的用戶則可忽略這一步。

   ```bash
   adduser [frappe-user]
   usermod -aG sudo [frappe-user]
   ```

2. 使用上一步建好的sudo使用者登錄系統，更新系統並重啟系統。

   ```bash
   sudo apt update && sudo apt upgrade -y && sudo shutdown -r now
   ```

3. 下載node.js

   ```
   curl -sL https://deb.nodesource.com/setup_18.x | sudo -E bash -
   ```

4. 安裝作業系統所需的各種依賴包

   ```bash
   sudo apt install -y python3.10-dev python3-setuptools python3-pip python3-distutils python3.10-venv software-properties-common mariadb-server mariadb-client redis-server nodejs xvfb libfontconfig libmysqlclient-dev nginx git ansible pkg-config libcairo2-dev libjpeg-dev libgif-dev librsvg2-dev
   ```

5. ~~將Python的pip源改成國內源，有助於後面安裝frappe時提高速度和成功率。~~

   ```bash
   pip config set global.index-url https://mirrors.aliyun.com/pypi/simple/
   pip config set install.trusted-host mirrors.aliyun.com
   ```

6. 接下來開始配置MariaDB，用nano編輯my.cnf文件。

   ```bash
   sudo nano /etc/mysql/my.cnf
   ```

   將游標移動到最後空白行，複製以下文本內容，粘貼後注意格式和換行要同下方，ctrl + X返回命令列，保存cy.cnf。

   ```bash
   [mysqld]
   character-set-client-handshake = FALSE 
   character-set-server = utf8mb4 
   collation-server = utf8mb4_unicode_ci 
   
   [mysql]
   default-character-set = utf8mb4
   ```

7. 重啟sql

   ```bash
   sudo service mysql restart
   ```

8. 開始mysql的安全配置

   ```
   sudo mysql_secure_installation
   ```

   第一個輸入資料庫密碼對話方塊出來的時候，直接敲回車代表沒有密碼，剩下的按照下面選擇：

   ```bash
   # 注：運行結果用 ··· 代替
   Enter current password for root (enter for none):  # 輸入root(mysql)的密碼，初次安裝預設沒有，直接回車 
    ... 
   Switch to unix_socket authentication [Y/n] n # 是否切換到unix通訊端身份驗證[Y/n]
    ... 
   Change the root password? [Y/n] y #是否設置root使用者密碼
   New password: # 新密碼
   Re-enter new password:  # 再次輸入密碼
    ... 
   Remove anonymous users? [Y/n] y # 是否刪除匿名使用者，建議刪除
    ... 
   Disallow root login remotely? [Y/n] n # 是否禁止root遠端登入，建議不開啟
    ... 
   Remove test database and access to it? [Y/n] n # 是否刪除test資料庫，可以保留
   ...
   Reload privilege tables now? [Y/n] y # 是否重新載入許可權表，也可以直接回車
    ... 
   Thanks for using MariaDB! # 看到這句話證明設置成功
   ```

9. 安裝yarn

   ```bash
   sudo npm install -g yarn
   ```

10. 查看版本，對照一下，這一步不做也行.

    ```bash
    node -v && npm -v && python3 -V && pip3 -V && yarn -v
    ```

11. 安裝bench，即erpnext系統的命令列管理工具，類似windows系統的程式管理器。

    ```bash
    sudo -H pip3 install frappe-bench
    ```

12. 使用bench命令安裝frappe框架。frappe-bench是安裝frappe框架的目錄名稱。

    ```bash
    bench init --frappe-branch version-15 frappe-bench --verbose
    ```

13. 再將安裝的系統使用者分配一下執行許可權。

    ```bash
    chmod -R o+rx /home/frappe/
    ```

14. 進入bench目錄

    ```bash
    cd frappe-bench
    ```

15. 新建網站，下面是以erpnext作為網站名稱。

    ```bash
    bench new-site erpnext
    ```

16. 設置為生產環境，即用supervisorctl管理所有進程，使用nginx做反向代理。如果安裝只是為了做開發，可以跳過這一步。

    ```bash
    sudo bench setup production frappe
    ```

17. 下載app (注意：一次只能執行一行指令)

    ```bash
    bench get-app --branch version-15 payments
    bench get-app --branch version-15 erpnext
    bench get-app --branch version-15 hrms  
    ```

18. 安裝app (注意：一次只能執行一行指令)

    ```bash
    bench --site erpnext install-app payments
    bench --site erpnext install-app erpnext
    bench --site erpnext install-app hrms
    ```

19. 安裝完後可查看一下是否有活動的wokers，同樣的，如果沒開啟生產環境，這一步也可以略過。

    ```bash
    bench doctor
    ```

20. 查看所需的app是否安裝正確，可以用這個命令

    ```bash
    bench version
    ```

21. 最後解決可能存在PDF列印中文顯示亂碼所需要的工具

    ```bash
    wget https://gitee.com/qinyanwan/erpnext/releases/download/v13.29.0/wkhtmltox_0.12.6.1-2.jammy_amd64.deb
    ```

    ```bash
    sudo dpkg -i wkhtmltox_0.12.6.1-2.jammy_amd64.deb
    ```

    如果安裝提示有缺少依賴的錯誤，執行下面命令。

    ```bash
    sudo apt -f install
    ```

    現在，我們可以檢查wkhtmltopdf 庫是否正確安裝並確認是否為所需版本：

    ```bash
    wkhtmltopdf –version
    ```

    **顯示wkhtmltopdf 0.12.6 (with patched qt)即是正確版本**

22. 如匯出PDF亂碼，需要另外安裝字體
    ```bash
    sudo apt-get install ttf-wqy-zenhei -y
    sudo apt-get install ttf-wqy-microhei -y
    ```

23. 成功安裝後，要記得執行啟動命令(建議安裝中文版本)
   ```bash
    bench start
    ```

**其他**

漢化、當地語系化請登錄 https://gitee.com/yuzelin/ 按需安裝相關APP。
