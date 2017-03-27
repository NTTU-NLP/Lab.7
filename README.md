h2. 資料檔說明

解開 Dataset\ 目錄內的 ReachOut.zip 壓縮檔。
內含 1894 個檔案。每個檔案兩兩一組，以編號 138717 為例，其對應的 138717.txt 檔案內含如下資訊：

```
red	followupWorse

Author:
6315	MemphisBelle
red	followupWorse

LastEditAuthor:
6315	MemphisBelle
Star contributor

Subject:
Re: So what happened.....

Body:
The TV launch was a few weeks ago and it was awesome. One of the rare times in my life I was actually happy and feeling worthwhile....
```

* 第一行的 red 代表這篇文章應該要被分類為 red。
* Author: 代表發文的作者 ID
* LastEditAuthor: 代表上次修改的作者 ID
* Subject: 其後的文字敘述為發文的主旨
* Body: 其後的文字敘述為發文的內容。

h2. Lab 說明

撰寫一程式能產生 Weka 的 ARFF 檔，並自行定義與輸出如下的 ARFF 資料格式：

```
@relation YOUR RELATION NAME
@attribute Label {green, …}
@attribute token1 numeric
@attribute token2 numeric
@attribute token3 numeric
…
@data
{0 green, 1 1, 2 1, …}
{0 red, 5 1, 9 1, …}
…