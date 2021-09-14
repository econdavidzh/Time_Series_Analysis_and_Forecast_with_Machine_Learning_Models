# Time Series Analysis + Forecasting with Machine Learning Models


The Notebooks in this repository contain the Time Series Analysis and ML Models to forecast
the Colombian Energy Market Price. 

The first file starts obtaining the data from XM servers in real time, consolidates it, and 
creates the dataframe with the required information. The second one develops a basic univariate
time series analysis identifying trend, seasonality and runing ADF test to determine whether the 
series is a stationary process.

The third file incorporates a multivariate in depth EDA, lagplots, autocorrelation and partial
autocorrelation functions as well as the required data transformation to correct non-stationarity
(which results are represented in the corresponding density function and qq-plots), to understand
the deterministic process of the autoregressive and moving average components of every series,
and estimates two Machine Learning Models: ARIMA and SARIMAX. The last one takes advantage of the 
multivariate EDA, and also is used to estimate the impulse-response functions that later are 
applyed to simulate future shocks which is an important improvement due to the fact that it is 
impossible for any model to anticipate unexpected changes.A fourth file contains the estimation 
and results of the Neural Prophet ML model.

The Notebook named **Eng Shock Simulations over Forecasting time series with multivariate impulse-response 
functions.ipynb** contains the functions and figures to simulate shocks, over the different independent 
variables, to determine the Energy price response according to the forecasts of the Machine Learning models.
