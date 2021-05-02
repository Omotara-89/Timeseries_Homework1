# Timeseries_Homework1
A Yen for the Future- prediction of the depreciation or appreciation of JPY aganist the CAD

In this assignment, is to test our understanding of the various time series tools learnt in order to predict future movements in the value of the Canadian dollar versus the Japanese yen.

After getting the csv file on the historical exchange rate betweem JPY and CAD, the dataset was trimmed to begin from January first 1990.

The price column was plotted to determine any pattern in the stated period. The plotted graph showed that despite the high volatility, JPY has been apprciating aganist the CAD and this shows a long-term strenghtening pattern.

The exchange rate price was later decomposed into trend and noise using the Hodrick-Prescott Filter.

Once the Hodrick-Prescott Filter was used to decompose the exchange rate price into two separate series and a dataframe was created, a graph plotting the Exchange Rate Price vs. the Trend for 2015 was presented.

This graph showed that there are little flunctuations when comparing the trend and the price lines. With this flunctuations, an abitrage oppotunity will exist for an active manager who can take advantage of this as a profitable trading opportunity in the shortrun.

The Arima Model was further used to determine if the p-value of the lags is a good fit or not. The result shows that the model is not a goof fit since its p-value is below 0.05

The garch model also showed that the 5 days forcast of volatility is predicted to increase.

For the Linear Regression forecast, a Scikit-Learn linear regression model was built to predict CAD/JPY returns with lagged CAD/JPY futures returns and categorical calendar seasonal effects.

To achieve thism the data was prepared and tested, predictions were made using the testing data and finanlly an out-of-sample and in-sample performance was used to determine if the model performed better or worse.
