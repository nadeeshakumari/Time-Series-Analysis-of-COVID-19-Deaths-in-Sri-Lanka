# 📈 Time Series Analysis of COVID-19 Deaths in Sri Lanka
This project performs time series analysis on daily COVID-19 deaths per million in Sri Lanka using ARIMA models in R. It includes data preprocessing, stationarity testing, model fitting with auto.arima, residual diagnostics, and forecasting.

## 📂 Project Structure
- **Dataset:** COVID-19 deaths in Sri Lanka

- **Script:** R Markdown file containing all analysis steps

- **Libraries Used:** forecast, tseries, lmtest, ggplot2, zoo, xts, dplyr, readr, scales

# 📊 Analysis Workflow
1. **Load and Visualize Data**
- Load the CSV dataset.
- Plot the raw data to explore the trend.

2. **Transform Data**
- Convert data into a time series object with daily frequency starting from October 22, 2020.

3. **Stationarity Check**
- Apply Augmented Dickey-Fuller (ADF) test.
- Difference the data if necessary to achieve stationarity.

4. **Model Identification**

- Examine ACF and PACF plots.

- Use auto.arima() to identify the best-fit model based on AICc.

5. **Model Diagnostics**

-Check residuals for autocorrelation using Ljung-Box test.

- Review residual plots.

6. **Forecasting**

- Forecast the future deaths for the next 10 periods.

- Plot forecast with 95% confidence intervals.

7. **Model Evaluation**

- Output forecasted values.

- Compute accuracy metrics.


