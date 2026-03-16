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

---

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

# 💡 Business Insights

Beyond the statistical modelling process, the analysis provides several insights that are relevant from a broader economic and business perspective.

**1. Inflation follows a persistent long-term upward trend**

The historical CPI data shows that inflation has generally increased steadily over the past three decades.  
This highlights how inflation gradually reduces purchasing power over time, which is an important consideration for businesses when planning pricing strategies, wage adjustments, and long-term investments.

**2. Inflation tends to change gradually rather than abruptly**

The strong dependence between CPI values across periods suggests that inflation evolves progressively rather than experiencing sudden shifts.  
For policymakers and financial institutions, this means that monitoring recent inflation data can provide useful signals about near-term economic trends.

**3. Forecast results suggest moderate inflation growth**

The forecasted CPI trajectory indicates that inflation is expected to **continue increasing at a moderate pace rather than accelerating sharply**.  
In practice, this implies a relatively stable inflation environment, where businesses and policymakers can anticipate gradual cost increases rather than extreme volatility.

**4. Data-driven forecasting supports economic decision making**

By combining statistical models with economic interpretation, forecasting tools like this can help governments, central banks, and organisations anticipate inflation trends and make more informed strategic decisions.

---

# 🌍 Project Impact & Applications

Although this project was developed in an academic setting, the forecasting approach reflects how data analytics can support real-world economic and business decision-making.

**1. Policy and economic analysis**

CPI forecasting plays a crucial role for central banks and policymakers when assessing inflation trends and determining monetary policy actions such as interest rate adjustments.

**2. Business planning and cost management**

For businesses, understanding expected inflation trends helps support decisions related to pricing strategies, budgeting, and long-term financial planning. Anticipating gradual increases in consumer prices can help companies better manage operating costs and maintain profitability.

**3. Financial market insights**

Investors and financial institutions closely monitor inflation forecasts when evaluating investment opportunities and portfolio risk. Reliable forecasts of inflation trends can support decisions related to asset allocation, bond yields, and interest-rate-sensitive investments.

**4. Data-driven economic decision making**

More broadly, this project demonstrates how statistical modelling and data analysis can be used to transform historical economic data into forward-looking insights that support informed decision making.

While simplified for academic purposes, the workflow in this project reflects the broader process used by analysts when building predictive models for macroeconomic indicators.
