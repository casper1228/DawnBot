# DAWN 驗證器擴充自動聲明
 Python 版的 Dawn Validator Bot

## 需要什麼
- Python

＃＃ 特徵

- 自動發送保持活動請求以獲取積分。
- 多重帳戶。
- 自動循環。
- 代理支援。


## 安裝和設定

＃＃＃ 安裝
1.克隆項目並進入項目目錄
   ```
   git clone https://github.com/casper1228/DawnBot.git
   ```
   ```
   cd DawnBot
   ```
2. 安裝所需的套件
   ```
apt install python3-requests
   pip install -r requirements.txt
   ```
### 設定並運行

1. 登入/註冊 Dawn Validator 帳戶並登錄，在瀏覽器中檢查元素的網路標籤中的 "getpoint?appid=" -> "authorization:" 中取得令牌 
2. In `DawnBot` directory, 編輯並調整此行 `accounts.yaml` 
   ```
  	accounts:
 	  - email: "account1@example.com"      # Replace with actual email
   	    token: "example_token_1"    # Replace with actual token
  	  - email: "account2@example.com"
   	    token: "example_token_2"
  	  # Add more accounts as needed
   ```
3. 編輯並調整此行 `config.yaml` 用於代理和延遲選項
   ```
	useProxy: false          # 如果要使用代理，則設為 true，否則設為 false
  	accountDelay: 121        # 處理每個帳戶的延遲（以秒為單位）
  	restartDelay: 241        # 重新啟動處理循環的延遲（以秒為單位）
   ```
4. 編輯 `proxy.yaml` 如果你想使用代理
5. 運行腳本來啟動，使用：
   ```
   python main.py
   ```
	
	
	
Dawn Validator Extension : https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp?authuser=0&hl=en


