# 資料檔說明

Dataset 目錄內 creatinine_training.txt 檔案為實驗資料，其中每行代表一個 training instance。
每一行的屬性以 tab 符號（\t）分隔。以第一行為例，其內含如下資訊：

```
102	Dr. Aldridge has been following this area and he will continue to follow-up with him . A1c , CBC , Fe , TIBC , ferritin , SGOT , SGPT , alkaline phosphatase , Bili T / D , TSH , Electrolytes , BUN / Creatinine , spot urine for microalbumin and creatinine 	Male	False
```

* 第一個屬性 102 代表這篇文章的 ID（應該要過濾掉，不納入特徵）。
* 第二個屬性為文字內容：代表內文
* 第三個屬性為該內文提及的個體所屬性別
* 最後一個屬性為答案

# Weka ARFF 檔輸出

撰寫一程式能產生 Weka 的 ARFF 檔，並自行定義與輸出類似如下的 ARFF 資料格式：

```
@relation YOUR RELATION NAME
@attribute Label {False, …}
@attribute token1 numeric
@attribute token2 numeric
@attribute token3 numeric
…
@data
{0 False, 1 1, 2 1, …}
{0 False, 5 1, 9 1, …}
…
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
