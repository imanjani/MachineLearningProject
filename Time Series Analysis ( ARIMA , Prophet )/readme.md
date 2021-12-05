# Forecasting-Bitcoin-Prices (ARIMA, XGBoost, Prophet, LSTM)
Forecasting Bitcoin Prices via ARIMA, XGBoost, Prophet, and LSTM models in Python.
Description: In this repo, I will test the Bitcoin forecasting abilities of 4 different Machine Learning models in Python: ARIMA, Prophet, XGBoost, and LSTM. By splitting the data into a testing and training set, I will compare each model’s performance with one another and conclude which performed best.


## Stationarizing the Dataset

Now, in order to produce good results from our Statistical ARIMA model, we need to stationarize our dataset. This data pre-processing work can be done by performing various transforms on our dataset. Moreover, in order to validate whether our dataset is stationary or not, we have used Dickey–Fuller test. 
Dickey–Fuller test tests the null hypothesis that a unit root is present inan autoregressive model. The alternative hypothesis is different depending on which version of the test is used, but is usually stationarity or trend-stationarity.

In order to stationarize the dataset, we have used a variety of transforms. We can use many transform like Cox-Box, Seasonal differentiation, and Regular Differentiation for this purpose. In our research, we applied them in the sequence mentioned above and we were able to successfully Stationarize our dataset with a Dicky Fuller test.

### Training ARIMA model

The statistical ARIMA model, accepts 3 parameters which are defined below,
1) *Lag Order (p)*- Number of lag observations included in the model
2) *Degree Of Differencing (d)*- Number of times that the raw observations are differenced
3) *Order Of Moving Average (q)*- Size of the moving average window 

In order to get the best model for our research, we trained our model for various values of (p,d,q) and then chosen the model according to AIC value. 

Akaike Information Criterion (AIC) is an estimator of the relative quality of statistical models for a given set of data. Given a collection of models for the data, AIC estimates the quality of each model, relative to each of the other models. Thus, AIC provides a means for model selection.

Given a set of candidate models for the data, the preferred model is the one with the minimum AIC value. Thus, AIC rewards goodness of fit, but it also includes a penalty that is an increasing function of the number of estimated parameters. The penalty discourages overfitting, because increasing the number of parameters in the model almost always improves the goodness of the fit.
Hence, the trained model for our research has the lowest Akaike Information Criterion value.


The datan.csv contains the bitcoin price table (closing price in USD) for a priod od 3 years,

---

# SARIMAX model 
### Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors
Most of Time-Series models consider past values of a dataset and past errors to determine future trends, seasonality and forecasted values. We look now to models that encompass these non-seasonal (p,d,q) and seasonal (P,D,Q,m) factors, but introduce the idea that external factors (environmental, economic, etc.) can also influence a time series, and be used in forecasting.
