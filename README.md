# Unit 10—A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.






- - -

### Files

We performed Time Series modeling and Linear Regression on Japanese Yen data


- - -

### Instructions

#### Time-Series Forecasting

In this notebook, we loaded historical Dollar-Yen exchange rate futures data and applied time series analysis and modeling to determine whether there is any predictable behavior.
And we found: 
ARMA model shows negative returns while ARIMA forecasts increase in price; The ARMA model AIC and BIC is lower, which should make this a better model, therefore I would not buy right now. The beta in Garch which signifies volatility is significant, therefore risk would be increased
I would not feel confident using these models for trading.



#### Linear Regression Forecasting

In this notebook, we built a Scikit-Learn linear regression model to predict Yen futures ("settle") returns with *lagged* Yen futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

We found that this is a good model because out of sample RMSE and in sample RMSE are fairly close, and the RMSE is low.  The fact that out of sample data RMSE or data the model has not seen before , was lower,it tells us that this can predict fairly well.

