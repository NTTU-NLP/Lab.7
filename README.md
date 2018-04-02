# 資料檔說明

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

# Weka ARFF 檔輸出

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
```

下面是實際的範例：

```
% Input
% Re : TwittRO It 's not fair @Sophie-RO
%
@relation 範例

@attribute Label {green, xxxx}
@attribute Re numeric
@attribute : numeric
@attribute "TwittRO" numeric
@attribute "It" numeric
@attribute "'s" numeric
@attribute not numeric
@attribute fair numeric
@attribute @Sophie-RO numeric

@data
{0 green, 1 1, 2 1, …}
...
```

# 使用 Weka 進行實驗

利用 Weka 的 Explorer 搭配使用 Decision Tree, SMO, SimpleLogistic 演算法進行 10 fold Cross-validation 來測試你跑的模型的正確率。

# 計分表

|評分項目|5|4|3|2|1|
|-|-|-|-|-|-|
|程式結果正確性||||||
|程式碼完整性||||||
|準時繳交||||||

# 分數
