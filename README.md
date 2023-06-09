# Bootstrap5 - 練習使用Sass變數開發網頁


* 加入Sass
* 製作Header首圖
* 製作主要內容
    * 自我介紹欄
    * 卡片式文章的使用
* 製作Footer及頁底聯絡表單樣式

---
## 加入Sass

先一如往常的將一開始需準備的東西加進網頁資料夾，如:
* 先做出基本的index網頁
* npm init 創出一個Project來管理
* npm i bootstrap 於Project中安裝bootstrap套件

再來就是將於資料夾中新增一個stylesheet資料夾用於存放後續的Sass/SCSS檔，並將VScode的Live Sass Compiler開啟讓我們產出的all.scss可以被自動編譯成網頁能取的all.css。

之後將bootstrap的_variables及_utilities另存塞進去另外創建的helpers資料夾方便管理，及把其他相關需要的bootstrap組件(包含前面被額外塞進helpers的檔案)給放進all.scss中。

---

## 製作Header首圖

圖片採用了 unsplash.com 的圖片
https://unsplash.com/photos/NWJzBizR3HI

主要以bs的排版將圖片置於中間，並於左上及右下做出了一個box並設定了其樣式。
中途也學習了修改bs的顏色規則，把 $primary 及 $secondary 的顏色做了修改。

---

## 製作主要內容
* 自我介紹欄

    圖片採用了 unsplash.com 的圖片，與header的圖片同作者
    https://unsplash.com/photos/ZXcYiPtCXIg
    
    這次一樣使用bs的排版來做圖片與文字的排版，但也學到了如果在手機版與電腦版的頁面切換中更改圖片的位置與順序。

* 卡片式文章的使用

    圖片一樣也是採用了 unsplash.com 的圖片

    使用bs的card樣式來建立卡片式文章的顯示，並學習了css的漸層設定方式與如何固定圖片尺寸。
    
    但這裡與範例有稍微弄的不太一樣，因為發現三張卡片在畫面小到一個程度時裡面的字會跑版突到卡片外，最後試了一陣子改成在斷點md時加入了卡片排版為二張的設定，而原本3張卡片的設定斷點則加到了斷點lg，來避免跑版問題。

---

## 製作Footer及頁底聯絡表單樣式

最後是試著使用額外套上bootstrap icon的CDN連結進頁面中，並以這些icon來做個人的聯絡方式及社群的id分享。

右側則是留言聯系，試著照老師影片中的格式去做了一樣的form。

後續套用的是bs本身的valid及測試按下送出時是否有出現訊息。