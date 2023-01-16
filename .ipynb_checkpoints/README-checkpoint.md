# FX_Master

![](images/readme-image.jpg)

*Image Source: https://www.forbes.com/fintech/2021/#9ba2c8731a63*

> FinTech Project 2

### Group Members

Pauline Liu, Flora Zhao and Md Muhasenul Haque

## Instructions on How to Read Through the Work

**1.** **Please begin with the jupyter notebook file titled "fx master" which contains the retrospective analysis which has been conducted using historical data**

**2.** **Then, please access the jupyter notebook file titled "MonteCarlo_Interactive" which is an interactive Monte Carlo Simulator using pandas data-reader**

**3.** **The presentation may be found under the filename "Presentation.pptm"**

**4.** **Finally, we wanted to incorporate the Python 'Panels' library into our code however were unable to do so due to time contraints, and so we have instead included the headway we've made so far. While it is not a comprehensive analysis, it does display the functionality of the Panels library and may be found as the jupyter notebook file titled "Crypto_Dashboard"**

*All jupyter notebook files may be found in the subfolder titled "codes"*

## Introduction

An exchange rate is a rate at which one currency will be exchanged for another currency and affects trade and the movement of money between countries.

Exchange rates are impacted by both the domestic currency value and the foreign currency value.

The exchange rate between two currencies is commonly determined by the economic activity, market interest rates, gross domestic product, and unemployment rate in each of the countries. Commonly called market exchange rates, they are set in the global financial marketplace, where banks and other financial institutions trade currencies around the clock based on these factors. Changes in rates can occur hourly or daily with small changes or in large incremental shifts.

### Motivation

This project is movitated by analysing different factors that may influence the fx rates, and try to use machine learning models to predict the moving direction of the exchange rate.

### Goals

* **Different factors that may influence the fx rates**

* **Predicting the moving directions of the fx rates using machine learning models**

* **different model comparisions on the performance/accuracy**


## Conclusions / Results

### The Ideal Cryptocurrency Portfolio

We decided that, at least at the level of the portfolios' composition, it would be best to select coins that have a large market cap as this would ensure that volatility is less than other less 'stable' coins, and would thus be the safer option.

The coins that we arrived at were;

* ```BTC``` **or Bitcoin**

* ```ETH``` **or Ethereum**

* ```BNB``` **or Binance**

* ```XRP``` **or Ripple**

* ```ADA``` **or Cardano**

* ```SOL``` **or Solana**

### The Monte Carlo Simulation as a tool for Cryptocurrency Forecasting

We found through our testing that while a MCS can be quite an effective tool for forecasting the potential price fluctuations of traditional stocks and equities, this applicability does not necessarily translate over to the cryptoverse. Through application of the interactive program that we developed, we found that the predictions had a variablity that was so vast that no meaningful conclusions could be drawn.

It became clear that due to the close-to exponential nature of cryptocurrency price growth over its entire history, retrospective analyses become severely skewed to expect similar price movements going into the future, and while such activity could arguably be a possibility, it's obvious that far more sophisticated techniques are required to meaningfully predict price movements in this space.

![](images/MCS_Output.png)

### Dollar-Cost Averaging vs Initial Lump-Sum Investment

We were very surprised to discover that what may seemingly appear to be a worthwhile investment strategy in traditional use cases, i.e. Dollar-Cost Averaging (where you invest into an equity/stock incrementally over time as opposed to all at once), such techniques proved to not be so fruitful in the domain of cryptocurrency investment.

The numbers were crunched, and the determination was made that you are infact much better off investing in crypto all at once with a lump-sum investment rather than incrementally over time. This analysis was done using historical data, and the supposition was such that an investor in the past would have invested in a cryptocurrency in one go, versus investing slowly over time as we cannot at this stage accurately project how such investment would look into the future.

Lump sum was found to trump DCA 80% of the time with the coins that we selected, with only ETH showing that DCA could have been an effective investment strategy. This comparison could have also been more comprehensive if we compared the sharpe ratios against the coins' standard deviations, thus taking risk factors into consideration, however we were unable to cover these in this project due to time contraints.

The plots that were generated during these analyses are as follows:

![](images/crypto_price_history.png)

![](images/crypto_daily_return.png)

![](images/crypto_cumulative_return.png)

![](images/crypto_standard_deviation.png)

![](images/crypto_sharpe_ratio.png)

![](images/DCA_vs_LumpSum.png)

## API and New Library

#### We used Pandas Data-Reader which is both an API and a new Library

## References

* **1** [6 Factors That Influence Exchange Rates](https://www.investopedia.com/trading/factors-influence-exchange-rates/)

* **2** [What Indicators Are Used in Exchange Rate Forecasting?](https://www.investopedia.com/ask/answers/021715/what-economic-indicators-are-most-used-when-forecasting-exchange-rate.asp)

* **3** [3 Examples of How Unemployment Rates Impact Currency Prices](https://www.valutrades.com/en/blog/3-examples-of-how-unemployment-rates-impacts-currency-prices)

* **4** [Australian Bureau of Statistics Unemployment Data and Statistics](https://www.abs.gov.au/statistics/labour/employment-and-unemployment/labour-force-australia/nov-2022#unemployment)

* **5** [Exchange Rate Prediction: Machine Learning with 5 Regression Models](https://towardsdatascience.com/exchange-rate-prediction-machine-learning-with-5-regression-models-d7a3192531d)

* **6** [Monthly Consumer Price Index Indicator](https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/monthly-consumer-price-index-indicator/latest-release)

* **7** [Federal Funds Rate - 62 Year Historical Chart](https://www.macrotrends.net/2015/fed-funds-rate-historical-chart)

* **8** [Consumer Price Index, Australia](https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/consumer-price-index-australia/latest-release)

* **9** [US Bureau of Labor Statistics Data CPI](https://data.bls.gov/timeseries/CUUR0000SA0&amp;amp;amp;output_view=pct_1mth)

* **10** [Ticks Volumns](https://forums.babypips.com/t/oanda-trading-volume/84294)

* **11** [Forex Data API](https://tradermade.com/forex)

* **12** [Change monthly data to daily in pandas](https://stackoverflow.com/questions/66759539/change-monthly-data-to-daily-in-pandas)

* **13** [Tutorial on Pandas Data-Reader](https://thecleverprogrammer.com/2021/03/22/pandas-datareader-using-python-tutorial/)

* **14** [Multiple Linear Regression With scikit-learn - GeeksforGeeks](https://www.geeksforgeeks.org/multiple-linear-regression-with-scikit-learn/)

* **15** [the difference between random_state = 0 & random_state = 1 | Data Science and Machine Learning](https://www.kaggle.com/discussions/getting-started/102258)

* **16** [Time Series Talk : ARIMA Model](https://www.simplilearn.com/top-python-libraries-for-data-science-article#8_pytorchhttps://www.youtube.com/watch?v=3UmyHed0iYE)

* **17** [statsmodels.tsa.arima.model.ARIMA](https://www.statsmodels.org/dev/generated/statsmodels.tsa.arima.model.ARIMA.html)

* **18** [AUD vs. US Dollar Index](https://en.macromicro.me/collections/345/mm-aud/18739/aud-dxy)

* **19** [Drivers of the Australian Dollar Exchange Rate](https://www.rba.gov.au/education/resources/explainers/drivers-of-the-aud-exchange-rate.html#:~:text=Australia%20has%20a%20floating%20exchange,in%20the%20foreign%20exchange%20market.)

* **20** [The Commodity Price and Exchange Rate Dynamics](https://www.scirp.org/journal/paperinformation.aspx?paperid=79731)

* **21** [Index of Commodity Prices](https://www.rba.gov.au/statistics/frequency/commodity-prices/2021/)

* **22** [How to Calculate Compound Investments Semi-Annually](https://budgeting.thenest.com/calculate-compound-investments-semiannually-26842.html)

* **23** [Historical inflation rates for United States of America](https://www.rateinflation.com/inflation-rate/usa-historical-inflation-rate/)

* **24** [Exchange Rate Prediction (Part 1): EDA & Data Visualisation](https://medium.com/analytics-vidhya/exchange-rate-prediction-part-1-276b6cd5338)

* **25** [Exchange Rate Prediction: Time Series Forecasting with ARIMA](https://medium.com/towards-data-science/exchange-rate-prediction-time-series-forecasting-with-arima-27260faafcdc)

* **26** [Top 10 Binary Classification Algorithms a Beginner’s Guid](https://towardsdatascience.com/top-10-binary-classification-algorithms-a-beginners-guide-feeacbd7a3e2)

* **27** [Classification: ROC Curve and AUC](https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc)

* **28** [How to Plot a ROC Curve in Python (Step-by-Step)](https://www.statology.org/plot-roc-curve-python/)













---







*Presentation Image References*

* **1** [BTC Coin](https://www.barrons.com/articles/things-to-know-today-51666952850)

* **2** [ETH Coin](https://www.dmarge.com/ethereum-price-prediction-aud)

* **3** [BNB Coin](https://play.google.com/store/apps/details?id=com.binance.dev&hl=en_AU&gl=US)

* **4** [XRP Coin](https://cryptomode.com/3-reasons-to-use-the-xrp-toolkit-when-interacting-with-the-xrp-ledger/)

* **5** [ADA Coin](https://www.newsbtc.com/analysis/ada/why-cardano-ada-may-breakout-in-a-bull-run-to-1/)

* **6** [SOL Coin](https://coinmarketcap.com/currencies/solana/)

* **7** [Mountain](https://i.pinimg.com/originals/1d/3f/43/1d3f4336e6d4d0b3bf9b1d42948db42c.jpg)

---

*Dec 26th 2022*

---