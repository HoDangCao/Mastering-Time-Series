# Time Series Data Analysis and Forecasting

This project provides a comprehensive approach to **exploring**, **analyzing**, and **forecasting** time series data. Through this repository, you'll find codes and insights covering essential properties, exploratory analysis, and forecasting techniques, with specific focus areas on detecting patterns, handling outliers, and engineering features for machine learning.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Characteristics of Time Series Data](#characteristics-of-time-series-data)
3. [Types of Time Series Data](#types-of-time-series-data)
4. [Outlier Detection](#outlier-detection)
5. [Seasonality & Trend Analysis](#seasonality-and-trend-analysis)
6. [Missing Data Handling](#missing-data-handling)
7. [Moving Average Smoothing](#moving-average-smoothing)
8. [Seasonal Decomposition & Differencing](#seasonal-decomposition-and-differencing)
9. [Forecasting Methods](#forecasting-methods)
10. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)

---

## Project Overview
Time series data represents observations collected sequentially over time and is highly applicable in various fields, including finance, energy, and economics. This project aims to streamline the time series exploratory data analysis (EDA) process, making it easier to uncover underlying patterns, trends, and seasonality. Our template provides a structured approach to EDA, pattern detection, and data preprocessing for model readiness.

## Characteristics of Time Series Data
- **Trend**: The direction of change in data values over time.
- **Seasonality**: Recurring cycles or patterns, such as weekly or monthly fluctuations.
- **Cyclic Patterns**: Non-fixed, recurring cycles over time, which differ from seasonality in regularity.

## Types of Time Series Data
- **Univariate**: One variable recorded over time (e.g., daily stock prices).
- **Multivariate**: Multiple variables recorded over time (e.g., stock price, volume, and volatility).
- **Regular vs. Irregular**: Time intervals between observations can be consistent (hourly, daily) or inconsistent.

## Outlier Detection
Outliers often emerge from sudden events (e.g., economic shocks, natural disasters). Outliers are identified through:
- **Visual Inspection**: Using line plots or box plots for quick identification.
- **Quantitative Analysis**: Defining specific outlier criteria based on distribution.

## Seasonality and Trend Analysis
Patterns over time are crucial for reliable forecasting. Key methods include:
1. **Visual Observation**: Analyze patterns over long periods to discern trends.
2. **Autocorrelation**: Evaluate self-correlation at different lags.

## Missing Data Handling
Two main methods are:
1. **Linear Interpolation**: Interpolates missing values within a range.
2. **Extrapolation**: Estimates missing values beyond the observed data range.

```python
# Linear Interpolation Example
import pandas as pd
data.interpolate(method='linear', inplace=True)
```

## Moving Average Smoothing
Moving averages help smooth data, reducing noise and highlighting trends:
- **Simple Moving Average (SMA)**: Assumes equal weights for past values.
- **Exponential Weighted Moving Average (EWMA)**: Assigns greater weights to recent data.

## Seasonal Decomposition and Differencing
Decomposition separates the data into:
- **Additive Model**: For stable variance.
- **Multiplicative Model**: For data with increasing variance.

```python
# Differencing Example
data_diff = data.diff(periods=1)
```

## Forecasting Methods
### Classical Methods
- **Moving Average (MA)**, **Autoregressive (AR)**, **ARIMA**
- **Seasonal ARIMA (SARIMA)**: Extends ARIMA to handle seasonality.

### Machine Learning Approaches
- **Linear Regression, Random Forests, Neural Networks (RNN, LSTM)**

## Exploratory Data Analysis (EDA)
### EDA Steps:
1. **Descriptive Statistics**: Summarizes central tendencies and dispersion.
2. **Time Plot**: Observes data points over time.
3. **Seasonal Plots**: Identifies recurring patterns within periods.
4. **Box Plots**: Highlights data distribution and outliers.
5. **Decomposition**: Splits data into trend, seasonality, and residuals.
6. **Lag Analysis**: Examines autocorrelations to detect trends and seasonality.

---

## Visual Examples
- **Seasonal Plot**: Visualizes seasonal effects over time.
- **Box Plot**: Depicts data distribution, highlighting potential outliers.
- **Autocorrelation Plot (ACF)**: Shows correlation between time-lagged data.

## Installation & Setup
To use this code:
1. Clone the repository: 
   ```bash
   git clone https://github.com/HoDangCao/Mastering-Time-Series.git
   ```
2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
The notebooks provides reusable functions, templates and detailed documentation for time series analysis and forecasting.

---

Let me know if you'd like adjustments to this README!
