# Time Series Forecasting

## Time Series Forecasting with ARIMA and SARIMA on Airline Passenger Data

This project explores time series forecasting using classical statistical models: ARIMA and SARIMA, on the well-known Airline Passenger dataset, which records monthly international airline passenger counts from 1949 to 1960. The dataset exhibits clear trend and seasonality, making it ideal for demonstrating time series decomposition, stationarity testing, differencing, and model fitting.

The core objective was to analyze the data, make it stationary, identify appropriate model parameters, and build predictive models to accurately forecast future passenger numbers. Both ARIMA (handling trend and autocorrelation) and SARIMA (incorporating seasonal effects) models were applied, evaluated, and compared. The SARIMA model showed improved performance by effectively capturing the dataset's seasonal patterns.


### ✅ Key Highlights:

* **📌 Objective:**
  Forecast future airline passenger numbers by applying and comparing ARIMA and SARIMA models.


* **📊 Dataset & Exploratory Analysis:**

  * Used monthly airline passenger data (1949-1960).
  * Visualized clear upward trend and yearly seasonality.
  * Decomposed time series into trend, seasonal, and residual components.

* **📈 Stationarity Testing:**

  * Applied Augmented Dickey-Fuller (ADF) test to check stationarity.
  * Initial series was non-stationary; performed differencing to reduce trend and seasonality.
  * Settled on first differencing despite borderline stationarity to preserve data integrity.

* **🧪 Parameter Identification:**

  * Used ACF and PACF plots on differenced data to identify ARIMA parameters (p=2, d=1, q=2).
  * For SARIMA, applied seasonal differencing and analyzed seasonal ACF/PACF to select seasonal parameters (P=1, D=1, Q=1, seasonal period=12).

* **🧠 Model Building and Fitting:**

  * Fit ARIMA(2,1,2) and SARIMA(2,1,2)(1,1,1,12) models.
  * Evaluated model summaries, statistical significance of coefficients, and diagnostics.

* **🛠️ Forecasting Approaches:**

  * Conducted in-sample forecasting, rolling forecasting with retraining, direct multi-step forecasting.
  * Additionally, performed out-of-sample forecasting on future dates to test prediction ability of the model.
  * Visualized forecast results against actual data for performance assessment.

* **🎯 Outcome:**

  * ARIMA model provided reasonable forecasts but struggled to capture seasonality.
  * SARIMA model better captured seasonal effects, clearly resulting in more accurate and reliable forecasts.
  * Forecast visualizations included confidence intervals to express prediction uncertainty.
