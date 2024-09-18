# Time Series Analysis of Average Temperature Data

Aleksandra Kalisz  
Postgraduate Diploma in Science in Data Analytics  
National College of Ireland, Dublin

alexkalisz@gmail.com

This repository contains a comprehensive analysis of two time series datasets representing the average temperatures from January 1844 to December 2004. The analysis includes various modeling techniques such as ARIMA, SARIMA, and Holt-Winters methods for forecasting temperature trends.

## Overview

The primary objective of this project was to identify and implement suitable time series models to forecast monthly and yearly temperature data provided by the Climate Institute of the University of East Anglia. The analysis includes:
- Preliminary assessment of the data using visualizations and statistical tests
- Application of smoothing techniques and decomposition
- Building and evaluating multiple time series models: Mean, Naïve, Seasonal Naïve, Holt’s model, Holt-Winters method, ARIMA, and SARIMA
- Forecasting and comparing results with the actual data for 2004

## Data

The datasets used in this project are:
- **Yearly Temperatures:** 161 rows representing the average yearly temperature.
- **Monthly Temperatures:** 1932 rows representing the average monthly temperature.

## Methodology

1. **Preliminary Assessment:**
   - Conducted Dickey-Fuller tests to check for stationarity.
   - Plotted the time series to visualize trends and seasonality.
   - Created seasonal plots for a more in-depth understanding.

2. **Smoothing Techniques:**
   - Applied moving averages to smooth out fluctuations and identify trends.
   - Seasonal decomposition using both additive and multiplicative models.

3. **Time Series Models:**
   - Implemented various models including:
     - Mean, Naïve, and Seasonal Naïve
     - Holt's Model
     - Holt-Winters Method
     - ARIMA (Auto ARIMA and Seasonal ARIMA)
   - Conducted diagnostic tests (e.g., Ljung-Box test) to assess model performance.
   - Evaluated models using Root Mean Square Error (RMSE) and Mean Absolute Error (MAE).

4. **Forecasting:**
   - Split data into training and testing sets.
   - Used the models to forecast 2004 temperatures.
   - Compared forecasted values with actual data.

## Results

- The **Auto ARIMA** model was found to be the most suitable for yearly temperature forecasting, with an RMSE of 0.46.
- For monthly temperature forecasting, both **SARIMA** and **Holt-Winters** methods were found to be effective, with RMSE values of 1.1 and 1.2, respectively.
- Visual comparisons between predicted and actual data indicate the effectiveness of these forecasting models in capturing overall trends.

## Requirements

To run this analysis, you need to install the following Python packages:
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`
- `scipy`
- `sklearn`

You can install them using:
```bash
pip install pandas numpy matplotlib statsmodels scipy scikit-learn
