# How to use 

### step1 請先將所有執行格跑遍

### step2 修改第二格中**回測資產輸入**的asset，參照範例填入需要回測之資產 (以2330,0050,qqq為例) ，請至yahoo財經查詢股票代碼

```python
#輸入回測之資產 (需要至Yahoo財經查看代碼) (台灣上市資料是.tw 上櫃資料是.two)

##範例1
#asset = "1101.TW,1102.TW,1215.TW,3430.TWO"

##範例2
#asset = "QQQ,TQQQ,SPY"

##回測資產輸入
asset ="2330.TW,0050.TW,qqq"
```

### step3 若需要自訂各項資產權重，可以更動第二欄中Proportion，並依照範例填入值

```python
##權重分配(非必填) ，依照需要回測個數填入相加等於1之值 ,若填空會產出平均分配1組並另外隨機生成10組權重
#Proportion = [0.3,0.3,0.3,0.1] 若有四項資產則即前三檔占比0.3,第四檔占比0.1。
#Proportion = [0.2,0.2,0.2,0.2,0.1,0.1] 若有六項資產可參考此Proportion，算四項占比0.2，後兩項占比0.1

Proportion = []
```
### step4 若需要跑清大大擂台，執行資料夾當下會有大擂台用.csv，可以直接將此csv上傳大擂台使用

### step5 再將所有執行格子跑遍，就可以在**資產回測結果欄**得到結果

