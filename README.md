# Testback-ASX


## Background

Backtest is an interesting python tool I found on the internet. I did read some blogs about how to use testback on testing trading strategy. This library contains many indicators and analysis tools which are commonly used in our trading accounts like MACD,SMA, BollingerBands, etc..  

A report released from the government of Western Australia shows that 47% of their financial year's GDP comes from the mining industry. Therefore, I would analyze the top 3 mining stocks,<b>RIO</b>,<b>FMG</b>,and <b>BHP</b>.  

Furthermore, I am also curious with bank stocks so I would analyze bank stocks as well.  

## Source

The stock data sets all sources from yahoo finance.       

## Process Of Analysis

Step 1. Use 22 years trading data to complete this Analysis. The first 20 years (2000.1.1 ~ 2019.12.31) will be the test period to structure mine strategy.Then use the strategy to test in the past 2 years (2020.1.1 ~ 2022.9.21). The reason is that I am going to use SMA as my trading signals and the SMA method does have the lagged effect when people use them to execute their trades.  

Step 2. Use yfinance library to source stock data with the timeframes I am interested in.    

Step 3. Transform datasets as csv files.  

Step 4. Use For-Loop method to run cerebro to find out the best match of short SMA and long SMA.  

Step 5. Use that best match to run the same process but applying the different time period which is (2020.1.1 ~ 2022.9.21) in this case.  

Step 6. Plot the results and display how much I can earn if I use that best match. 

<img src='https://github.com/LynHJ/ProjectTestback/blob/9fdee4201fd7f0a0f720a55ec550851ce5a1885b/OutputData/FMG.AX.png' width= 50% height=50%/> <img src='https://github.com/LynHJ/ProjectTestback/blob/9fdee4201fd7f0a0f720a55ec550851ce5a1885b/OutputData/RIO.AX.png width= 50% height=50%/> 
 



## Summary
1. The idea of using 20years-2years to run the strategy is that we encountered a financial crisis in 2008 and we have been through a covid period which hit gobal econimic hard. So if during the this down-award trenth, I still can get positive profit then I reckon my strategy is good to go.  

2.  This process still has some defect.For example, to form up a great strategy is not just using two numbers to produce trading signals, and the earning of target mining companies actually depend on the demands from China,.etc.


## Content:
```
Project  


```

## Installation

pip install -r requirements.txt


## Reference

1. https://www.google.com.au/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwisu4-U-9n6AhVFw3MBHdxpC5oQFnoECA4QAw&url=https%3A%2F%2Fwww.wa.gov.au%2Fsystem%2Ffiles%2F2021-12%2FWA%2520Economic%2520Profile%2520-%2520November%25202021.docx&usg=AOvVaw1ECnCOvex93CDjUBnwmKsC  
2. https://www.finlab.tw/python：vix美股大跌投資法/
3. https://codeantenna.com/a/uI1mLI5E4F





 
