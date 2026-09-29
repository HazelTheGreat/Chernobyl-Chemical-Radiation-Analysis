# Chernobyl Chemical Radiation Analysis

This repository contains statistical analysis, exploratory data visualization, and predictive modeling of chemical and radiological measurements in the Chernobyl area using Multiple Linear Regression (MLR).

## Abstract

Evaluating environmental radiation hazards requires understanding the relationship between chemical markers and radiation levels. This project applies multivariate statistical modeling to analyze environmental sampling data from Chernobyl. By constructing and evaluating a Multiple Linear Regression (MLR) model, the study assesses how various chemical parameters influence radiation concentrations and provides rigorous diagnostic testing to validate model performance and classical linear regression assumptions.

## Authors & Contributors

* **Hazel Zaki Adityo** — NIM: 2702329576 — [@HazelTheGreat](https://github.com/HazelTheGreat)
* **Anthony** — NIM: 2702377612
* **Satya Darma Padmakumara** — NIM: 2702244662

## Objectives

1. **Exploratory Data Analysis:** Examine distributions, variance, and correlation patterns among chemical predictors and radiation metrics.
2. **Predictive Modeling:** Construct a Multiple Linear Regression model to quantify the relationship between independent chemical factors and dependent radiation parameters.
3. **Diagnostic Checking:** Validate linear regression assumptions, including normality of residuals, homoscedasticity, absence of multicollinearity, and independence of errors.
4. **Performance Evaluation:** Measure predictive accuracy and goodness-of-fit using metrics such as $R^2$, Adjusted $R^2$, RMSE, and MAE.

## Methodology

1. **Data Preprocessing & Cleaning**
   * Inspection of missing values, outlier detection, and variable scaling.
   * Feature correlation analysis to screen for potential collinearity among predictors.

2. **Model Specification & Estimation**
   * Formulation of the Multiple Linear Regression model:
     $$Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \dots + \beta_k X_k + \epsilon$$
   * Parameter estimation using Ordinary Least Squares (OLS).

3. **Regression Diagnostics**
   * Variance Inflation Factor (VIF) testing for multicollinearity.
   * Shapiro-Wilk test for residual normality.
   * Breusch-Pagan test for heteroscedasticity.
   * Durbin-Watson test for autocorrelation.

4. **Model Evaluation & Interpretation**
   * Hypothesis testing ($t$-tests for individual predictors, $F$-test for overall model significance).
   * Assessment of coefficient weights and residual behavior.

## Tech Stack

* **Language:** R / Python
* **Libraries & Packages:**
  * `tidyverse`, `ggplot2` (Data manipulation & visualization)
  * `car`, `lmtest`, `MASS` (Linear regression diagnostics & hypothesis testing)

## Repository Structure

```text
Chernobyl-Chemical-Radiation-Analysis/
├── data/               # Sampling datasets and environmental measurements
├── scripts/            # R/Python scripts for EDA, data cleaning, and MLR modeling
├── reports/            # Research paper draft, presentation materials, and compiled reports
├── outputs/            # Exported diagnostic plots, regression summaries, and figures
└── README.md           # Main project documentation
