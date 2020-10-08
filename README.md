# RB-Code

## 2019 Codes:
### File used: 
#### "CrypotQuant_BTC_20190101-20200229.csv" 
### Graphs : 
#### 2019 Graphs.ipynb 
#### https://yxiao19.github.io/RedBlock/2019Graphs.html 
### LSTM Models on price_high_usd and price_low_usd (Blue and yellow lines are actua data, green is predicted)
#### 2019 LSTM Price (Only Price, train+test).ipynb
#### 2019 LSTM High-Low Price (Only Price, Low on High, High on Low).ipynb


## 2020 Codes:
### File used: "
#### CrypotQuant_BTC_20200301-20201004_Prices.csv"
### LSTM Models on predicting future price_high_usd (till 2020/12/31): (Blue is actual, green is the test dataset that’s predicted, orange is the predict of future price)
#### 2019 LSTM Predict Future Price (Only Price).ipynb
##### Train Data: price_usd_low (From 3/1/2020 to 10/4/2020)
##### Test  Data: price_usd_high (From 3/1/2020 to 10/4/2020)
##### Predict price_usd_high 10/5/2020 to 12/31/2020

##### Data selection: 
##### Used past 43-day price to predict future price. (Different from the timestamps we did before).

##### For the timestamp = 60, we are using price of day 1 to day 60 to predict price of day 61 and use price of day 2 to day 61 to predict price of day 62, so if we want to know the price of day t, we need to know the price of day t-1. Thus, we are not able to predict the price of 12/31/2020 if we only know the price from the past to 10/04/2020 because we actually need the price of 12/30/2020.

##### So to predict the price from 10/05/2020 to 12/31/2020 (88 days), I used the prices from 8/23/2020 to 10/04/2020 (43 days) to predict the price of 12/31/2020, the prices from 5/28/2020 to 07/09/2020 (43 days) to predict the price of 10/05/2020. 




