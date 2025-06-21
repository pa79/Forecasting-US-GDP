# 📈 Forecasting U.S. GDP Growth

## 🔍 Overview

This project aims to **forecast the quarterly growth rate of U.S. Gross Domestic Product (GDP)** for the **nine quarters following December 2019**. The project was designed in the context of pre-pandemic economic uncertainty, with many economists anticipating a potential recession by the end of 2020.

> 🗞️ *"According to a survey by the National Association for Business Economists, two-thirds of economists predicted a U.S. recession by the end of 2020."*  
>  
> 🗣️ *"The stimulus is going to hit the economy in a big way this year and next year, and then in 2020 Wile E. Coyote is going to go off the cliff."* — Ben Bernanke, former Federal Reserve Chairman (June 2018)

However, **no one foresaw the impact of a global pandemic**, which drastically altered the economic landscape. This project evaluates the predictive power of economic indicators **prior to the COVID-19 crisis**.

---

## 🧠 Objective

To build an econometric forecasting model that:

- Predicts U.S. GDP growth from Q1 2020 through Q1 2022
- Utilises an **Ordinary Least Squares (OLS) autoregressive model**
- Incorporates **macroeconomic indicators** that are historically predictive of GDP growth (e.g., unemployment, interest rates, stock indices, industrial production, consumer sentiment)

---

## ⚙️ Methodology

1. **Data Collection**
   - U.S. Real GDP growth data (quarterly)
   - Macroeconomic indicators from FRED and other sources
   - Time series up to Q4 2019

2. **Feature Engineering**
   - Lagged GDP growth terms (autoregressive structure)
   - Transformation and normalization of input indicators
   - Rolling means and quarterly aggregates as needed

3. **Model Development**
   - Baseline: OLS autoregressive model
   - Extended: OLS with additional predictive indicators
   - Model evaluated using:
     - Root Mean Squared Error (RMSE)
     - Mean Absolute Error (MAE)
     - Out-of-sample forecasting accuracy

4. **Forecasting**
   - Generate forecasts for 9 quarters beyond Q4 2019
   - Visualise prediction intervals and trend changes

---

## 📊 Tools & Libraries

- Python 3.x
- `pandas`, `numpy` for data manipulation
- `statsmodels` for OLS regression modeling
- `matplotlib`, `seaborn` for data visualization
- Data sourced from: [FRED](https://fred.stlouisfed.org/), BEA, OECD



