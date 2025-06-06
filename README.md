# 📈 Earnings Surprise Prediction – FP&A ML Pipeline with SHAP

A data-driven project that simulates a **Financial Planning & Analysis (FP&A)** use case: predicting whether **S&P 500 companies** will beat quarterly earnings expectations using public financial data and explainable machine learning.

> 🧠 **Use case**: Sell-side analysts, buy-side investors, and internal FP&A teams can use this model to anticipate earnings outcomes and improve forecast accuracy.

---

## 🧭 Project Overview

| Category | Details |
|----------|---------|
| 🎯 Objective | Predict if a company will report EPS > Estimate (binary surprise) |
| 🛠 Tools | Python, `yfinance`, `XGBoost`, `SHAP`, `scikit-learn`, `matplotlib`, `seaborn` |
| 📦 Dataset | S&P 500 companies' EPS Actual vs Estimate (2019–2024) |
| 📍 Output | Binary classification (`1 = beat`, `0 = meet/miss`) |

---

## 📂 Folder Structure

![PR Curve](https://github.com/Hanklin999/images/blob/main/Python_PR_Curve.png)

## Explainability – SHAP
SHAP plots revealed sector and quarter patterns influencing predictions.

![SHAP Sector](https://github.com/Hanklin999/images/blob/main/shap_sector_plot.png)

##  Files
- `earnings_surprise_colab.ipynb`: ![Full end-to-end pipeline](https://github.com/Hanklin999/Python_earnings-surprise-prediction/blob/main/earnings_surprise_prediction_colab.ipynb)

##  Appendix – Hyperparameter Tuning
Included sensitivity analysis on `scale_pos_weight` for XGBoost from 0.1 to 1.0
