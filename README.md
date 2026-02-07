# NLP_Project



Abstract
In this project, we analyze historical stock price data using time series modeling techniques, specifically Autoregressive (AR) and Moving Average (MA) models. Stock prices change over time based on past price movements and random market fluctuations.
The objective of this study is to understand the temporal behavior of stock prices by visualizing trends, testing stationarity, and analyzing autocorrelation patterns. Based on these observations, AR and MA models are applied to model short-term stock price movements. This project helps in understanding how past stock prices influence future prices and forms a foundation for financial forecasting.

Problem Statement
Stock price data is sequential and time-dependent in nature. Current stock prices are influenced by previous prices, market trends, and random disturbances. Without proper time series analysis, predicting stock prices can result in inaccurate outcomes.
The goal of this project is to statistically analyze stock price data to:
•	Identify price trends and fluctuations
•	Measure dependency on previous stock prices
•	Check stationarity of the data
•	Apply AR and MA models for stock price modelling

Objectives
•	To study historical stock price movements
•	To analyze autocorrelation and partial autocorrelation
•	To test stationarity of stock price data
•	To implement AR and MA models
•	To understand short-term stock price behavior

Dataset Description and Preprocessing
The dataset consists of historical stock market data, including attributes such as Date, Open, High, Low, Close, and Volume. For modeling purposes, the Closing Price is selected.
Preprocessing Steps:
•	Date column converted into datetime format
•	Date set as the time index
•	Missing values removed or handled
•	Data sorted chronologically

Time Series Visualization
A time series plot of stock closing prices is generated to observe price behavior over time.

Observations:
•	Stock prices show continuous fluctuations
•	Presence of upward and downward movements
•	Sudden changes indicate market volatility
•	This visualization helps in understanding the overall pattern of stock price movements.

Stationarity Testing
Stationarity is essential for applying AR and MA models. A stationary time series has constant mean and variance over time.

The Augmented Dickey-Fuller (ADF) test is used to check stationarity.

Interpretation:
•	p-value > 0.05 → Data is non-stationary
•	Stock price data is usually non-stationary due to trends
•	Hence, differencing may be applied before modeling.

Autocorrelation Function (ACF) Analysis
ACF measures the correlation between current stock prices and their past values.

Results:
•	High correlation at initial lags
•	Gradual decay of correlation
•	Indicates influence of past price movements
•	ACF helps in identifying the order of the MA model.

Autoregressive (AR) Model
The AR model predicts the current stock price using its previous price values.

Features:
•	Depends on lagged stock prices
•	Captures momentum in price movements
•	Suitable when PACF shows sharp cutoff

Moving Average (MA) Model
The MA model predicts stock prices using past error terms.

Features:
•	Models random market shocks
•	Smoothens noise in stock price data
•	Suitable when ACF shows sharp cutoff

Results and Discussion
•	Stock prices show strong dependency on past values
•	Non-stationarity is observed in raw data
•	ACF and PACF help in selecting AR and MA orders
•	AR and MA models effectively model short-term price behavior

Conclusion
This project demonstrates the application of AR and MA models for modeling stock price time series data. Understanding trends, stationarity, and autocorrelation patterns is essential for building accurate financial models. This study provides a strong foundation for advanced forecasting models such as ARIMA in stock market prediction.


 
 
 
 
 
 
 
 
 
