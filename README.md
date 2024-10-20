# Google Colab使用教學（附帶MINST案例）
## Google Colab使用教學（附帶MINST案例）
### Google Colab是什麼？
Google Colab是Google免費提供的Jupyter筆電環境，支援CPU、GPU和NPU處理，提供諸如TensorFlow、pytorch、Kernal等主流深度學習框架的環境。該平台部署在雲端，不影響本地使用，因此再拉比再垃圾的電腦也依舊能夠正常使用。<br>
Colab官網：https://colab.research.google.com/

#### 為什麼選擇該平台
Google Colab為所有的開發者免費提供一定的GPU算力，每個人大約能分到一張特斯拉T4顯示卡的算力，該顯卡單精度浮點運算能力大約在2070與1080之間，同時擁有16G顯存，如果自己擁有更好的顯示卡（如用4090的富哥）那用自己的會更好。若自己電腦為3060的，雖然單精度浮點運算能力比T4強，但出於顯存考量以及自己筆電經常外帶的需求，筆者建議使用該平台會更好。<br>
由於是免費提供的，因此該算力也有限制，即每週最多使用三十小時左右（大概，官方也沒有公佈限額，這是動態資源），同時單次運行不能超過12小時，同時若使用用戶過多的情況不一定能使用上。<br>
Colab Pro 訂閱者的使用量仍會受到限制，但相比非訂閱者可享有的限額要多出約一倍。 Colab Pro+ 訂閱者還可獲得更高的穩定性。

### Google Driver是什麼？
Google Driver是Google推出的線上儲存服務，類似百度雲端盤，目前有付費和免費兩種模式，免費用戶可享有15G的空間，付費用戶根據方案最多可享有20TB的空間。<br>
Google Driver：https://drive.google.com/drive/

#### 為什麼要使用該雲端盤
如上文所說，Google Colab是Google免費提供的Jupyter筆記本環境，那麼每次關閉該環境，伺服器會自動將之前的所有操作進行清除，若不使用Google Driver，則每次都需要上傳資料集和程式碼，大大浪費了時間，因此使用該雲端盤，和Colab進行連結操作，在使用Colab的時候可以呼叫網盤的數據

### 正式教學
#### 筆記本創建
首先進入Google Driver：https://drive.google.com/drive/
![image]()

點選左上角的新建-更多
![image]()

這時候你已經可以看到Google Colaboratory，若沒有則點擊“關聯更多應用程式”，搜尋“Colab”，安裝第一個即可

進入Colab

若直接點選Colab的網址則為該頁面

這時你只需要點擊左上角的文件-新筆記本便可以進到相同的頁面
左邊有五個選項，分別為目錄、查找和替換、變量、Secret（秘鑰）、文件
之後點擊代碼執行程序，然後點選更改運行時類型，在其中硬體加速器部分選擇GPU保存，Colab便會配置一個帶有GPU的機器，此時筆記本就創建完成了。

### 雲端硬碟掛載由於我們的資料集以及程式碼檔案都放在了Google雲端碟上，因此還需要對Google雲端硬碟進行掛載在新建立的筆記本中輸入以下程式碼

# 參考資料
[Google Colab使用教學（附帶MINST案例）]([https://blog.csdn.net/dawnlini/article/details/128236315](https://blog.csdn.net/sggrafaf/article/details/136657651?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-12-136657651-blog-138222764.235%5ev43%5econtrol&spm=1001.2101.3001.4242.7&utm_relevant_index=15))
