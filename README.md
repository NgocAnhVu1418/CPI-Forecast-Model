# CPI Forecast Model 📈

This project develops a **time series forecasting model for the Consumer Price Index (CPI)** using historical quarterly data from 1990 to 2022.

The objective is to build a predictive model capable of forecasting CPI values for the next **six quarters (Mar 2023 – Jun 2024)** and evaluate its accuracy using statistical metrics.

This project was completed as part of the **QBUS6840 Predictive Analytics course at the University of Sydney**.

---

# Project Overview

The **Consumer Price Index (CPI)** is one of the most important economic indicators used to measure inflation and changes in the cost of living.

Accurate CPI forecasting is important because it helps:

- central banks adjust monetary policy
- governments assess economic stability
- businesses anticipate changes in purchasing power

In this project, several forecasting approaches were explored and compared to identify the most suitable model for CPI prediction.

---

# Data

The dataset contains **quarterly CPI observations from March 1990 to December 2022 (132 data points)**.

Additional macroeconomic context is provided through **cash rate data**, which helps validate whether the predicted CPI trend is economically reasonable.

# 📊 Key Visualisations

Visual exploration plays an important role in understanding the behaviour of the CPI time series and validating the forecasting models used in this project.

---

## CPI Trend Over Time

The historical CPI data from 1990 to 2022 shows a clear **long-term upward trend**, reflecting persistent inflation over the past three decades.

While CPI growth remained relatively stable for many years, a noticeable acceleration occurred in the early 2020s. This pattern is consistent with global inflationary pressures following the COVID-19 pandemic, supply chain disruptions, and changes in monetary policy.

Understanding this trend is important because it highlights the **non-stationary nature of the CPI series**, which must be addressed before applying time series models such as ARIMA.

![CPI Trend](images/cpi_trend.png)

---

## Autocorrelation Structure of CPI

The **Autocorrelation Function (ACF)** plot reveals strong persistence in the CPI time series.

The slow decay of autocorrelation values suggests that CPI observations are highly dependent on previous periods, which is typical for macroeconomic indicators.

This behaviour confirms that the time series is **non-stationary**, supporting the use of **first-order differencing** before fitting ARIMA models.

![ACF Plot](images/acf_plot.png)

---

## CPI Forecast Results

Using the selected **ARIMA(2,1,0)** model, CPI values were forecasted for the next six quarters.

The forecast shows a **moderate upward trajectory**, suggesting that inflation is expected to continue rising gradually rather than accelerating sharply.

This result aligns with macroeconomic expectations under a relatively high interest rate environment, where monetary tightening typically slows down inflation growth.

![CPI Forecast](images/cpi_forecast.png)

---

## Key Takeaways from Visual Analysis

The visualisations highlight several important characteristics of the CPI series:

- CPI exhibits a **long-term upward trend** consistent with persistent inflation.
- The series demonstrates **strong autocorrelation**, indicating dependence between observations over time.
- Forecast results suggest **moderate and stable inflation growth** in the near future.

Together, these visual insights support the model selection and help connect statistical forecasting with real-world economic interpretation.
