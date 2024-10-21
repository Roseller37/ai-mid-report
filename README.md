# Google Colaboratory–適合Python初學者的雲端開發環境
### 簡介
Colaboratory (以下簡稱Colab)是一個在雲端運行的編輯執行環境，由Google提供開發者虛擬機，並支援Python程式及機器學習TensorFlow演算法。最棒的是只需要瀏覽器就可以運作，完全免費，目前官方建議使用Chrome，Firefox或Safari。

Colab目的在提供Machine Learning機器學習教育訓練及研究用，不須下載、不須安裝就可直接應用Python 2.7 與 Python 3.6資源庫，對初學者來說可以快速入門，不需耗時間在環境設定上。程式碼預設會直接儲存在開發者的Google Drive雲端硬碟中，執行時由虛擬機提供強大的運算能力，不會用到本機的資源。但要注意在閒置一段時間後，虛擬機會被停止並回收運算資源，此時只需再重新連接即可。接下來我們就來看操作環境：

### Colab Notebook環境介紹
開啟chrome先登入google帳號，連結URL https://colab.research.google.com/，出現對話窗如下，<br>
![image]()

按下右下角 NEW PYTHON 3 NOTEBOOK，出現如下的cell code區域。<br>
![image]()

點擊 code cell進入編輯模式並貼上這段python程式碼：

```
import numpy
import matplotlib.pyplot as plt

x = numpy.random.normal(5.0, 1.0, 100000)

plt.hist(x, 100)
plt.show()
```

按下左側執行button 或CTRL+Enter。會看到正態分布直方圖結果如下：<br>
![image]()

對了，Colab有code IntelliSense功能，以上述範例來說，在前面兩行import完numpy等函式庫後，請先按下執行。接著再寫 x= numpy.random.n…編輯器會自動顯示代碼完成，參數信息，快速信息和成員列表等功能，十分方便，如下圖。<br>
![image]()

將滑鼠移至code cell右上角RAM/Disk區域時，可以顯示本次執行虛擬機所分配的資源：約12GB RAM，100GB Disk，如下圖。<br>
![image]()

### 版本比較Revision History
點選工具列File -> Revision History，或直接於主工具列上按下All changes saved，有時會顯示Last saved at…(某時間點)。你會看到幾乎任何時間點的更動都被記錄下來，可以做檔案比較、選擇再次開啟歷史版本或復原版本。<br>
![image]()

### 於notebook (副檔名.ipynb)中任意加入code cell或text cell
由於Colab是基於Jupyter Notebook發展出來的互動式環境，可以任意加入code cell(使用Python和其他語言編寫和執行代碼)或text cell(使用稱為markdown的簡單標記語言進行格式化筆記)。在下圖中，「下面的global變數x值是由上面這個cell得來，且不用再import函式庫，即可畫出Scatter Plot。」這段敘述是在Text cell中，同樣用點擊區塊方式進入編輯模式。新增這些cells方式也很簡單，將滑鼠移到cell的上方或下方皆可。
![image]()

接下來編輯執行第二個cell code，程式碼如下：

```
y = numpy.random.normal(10.0, 2.0, 1000)

plt.scatter(x, y)
plt.show()
```

得到錯誤訊息如下圖：
![image]()

原來是x和y size必須相同。這是很容易修正的錯誤訊息，但是若一時看不出來問題在那兒呢？Colab在ValueError:下提供一個按鈕<br>
`SEARCH STACK OVERFLOW`，方便我們查詢網站stack overflow的相關解答，非常實用。修改後就可畫出正確分布圖形了：









# 參考資料
[Google Colaboratory–適合Python初學者的雲端開發環境](https://www.cc.ntu.edu.tw/chinese/epaper/0052/20200320_5207.html)
