# 📈 Time Series Analysis of COVID-19 Daily Deaths in Sri Lanka
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

Stationarity Check

Apply Augmented Dickey-Fuller (ADF) test.

Difference the data if necessary to achieve stationarity.

Model Identification

Examine ACF and PACF plots.

Use auto.arima() to identify the best-fit model based on AICc.

Model Diagnostics

Check residuals for autocorrelation using Ljung-Box test.

Review residual plots.

Forecasting

Forecast the future daily deaths for the next 10 periods (customizable).

Plot forecast with 95% confidence intervals.

Model Evaluation

Output forecasted values.

Compute accuracy metrics.

📦 Requirements
Ensure the following R packages are installed:

r
Copy
Edit
install.packages(c("forecast", "tseries", "lmtest", "ggplot2", 
                   "zoo", "xts", "dplyr", "readr", "scales"))
📁 Data Source
The dataset (srilanka.csv) should be placed at:

swift
Copy
Edit
C:/Users/ASUS/Desktop/Corona/srilanka.csv
You can modify the file path in the script to match your local directory.

🧪 Example Forecast Plot
The script ends with a forecast plot visualizing the predicted number of deaths per million with a 95% confidence interval.

📌 Notes
Time series frequency is set to 365 (daily).

ADF test is used for checking stationarity.

Model selection is based on KPSS test and AICc.

Only 10 future periods are forecasted — adjust h as needed for longer forecasts.
