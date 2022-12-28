# Tokyo_Stock_Exchange_Prediction

### Introduction: 
This dataset contains historic data for a variety of Japanese stocks and options. Your challenge is to predict the future returns of the stocks.

### Dataset: [Link](https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction/data)

### Metric: 

The model will use the closing price ( 𝐶(𝑘,𝑡) ) until that business day ( 𝑡 ) and other data every business day as input data for a stock ( 𝑘 ), and predict rate of change ( 𝑟(𝑘,𝑡) ) of closing price of the top 200 stocks and bottom 200 stocks on the following business day ( 𝐶(𝑘,𝑡+1) ) to next following business day ( 𝐶(𝑘,𝑡+2) )

                                                  𝑟(𝑘,𝑡)=𝐶(𝑘,𝑡+2)−𝐶(𝑘,𝑡+1)/𝐶(𝑘,𝑡+1)
 
Within top 200 stock predicted ( 𝑢𝑝𝑖(𝑖=1,2,…,200) ), multiply by their respective rate of change with linear weights of 2-1 for rank 1-200 and denote their sum.

Use the purchase minus the sell of stock as the daily return. For the given days, Get the mean of daily return divided by standard deviation of daily return. The higher the minus the better.
