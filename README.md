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
   pip install -r requirements.txt
   ```
### 設定並運行

1. Login/register Dawn Validator account and login, get the token in "getpoint?appid=" -> "authorization:" at network tab in inspect element in browser. 
2. In `DawnBot` directory, Edit and adjust this line in `accounts.yaml` and save it
   ```
  	accounts:
 	  - email: "account1@example.com"      # Replace with actual email
   	    token: "example_token_1"    # Replace with actual token
  	  - email: "account2@example.com"
   	    token: "example_token_2"
  	  # Add more accounts as needed
   ```
3. Edit and adjust the `config.yaml` for proxy and delay options.
   ```
	useProxy: false          # Set to true if you want to use proxies, false otherwise
  	accountDelay: 121        # Delay in seconds for processing each account
  	restartDelay: 241        # Delay in seconds for restarting the processing loop
   ```
4. Edit the `proxy.yaml` if you want to use proxy
5. Run the script to start, use :
   ```
   python main.py
   ```
	
	
	
Dawn Validator Extension : https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp?authuser=0&hl=en


