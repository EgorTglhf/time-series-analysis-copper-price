# time-series-analysis-copper-price

[This project](time-series-analysis-copper-price.ipynb) focuses on forecasting copper prices using time series analysis and machine learning models. Key steps included testing stationarity with the Augmented Dickey–Fuller test and removing trends by differencing. Seasonality was analyzed via decomposition and confirmed to have minimal influence using Autocorrelation and Partial Autocorrelation plots.

Four models were implemented:

1. Holt-Winters (Exponential Smoothing): Evaluated residuals for normality and no autocorrelation (Ljung-Box test).
2. Autoregression (AR): Used significant lags identified through Partial Autocorrelation of the differenced series.
3. ARIMA: Combined AR and MA for integrated time series, with significant lags chosen via Autocorrelation.
4. ARIMAX: Extended ARIMA by incorporating Fourier Series as exogenous features for Harmonic Regression.
