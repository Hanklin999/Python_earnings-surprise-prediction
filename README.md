# Python_earnings-surprise-prediction
A data-driven FP&amp;A project predicting earnings surprises using S&amp;P 500 data and SHAP-based model interpretation.

#  Earnings Surprise Prediction (S&P 500)

This project simulates a real-world Financial Planning & Analysis (FP&A) scenario by predicting whether a public company will beat earnings expectations using sector and quarter data.

---

##  Objective
- Predict `Reported EPS > Estimated EPS` (earnings surprise)
- Support earnings alert systems and forecast calibration

##  Tools
Python, pandas, yfinance, scikit-learn, XGBoost, SHAP, seaborn, matplotlib

## Model Comparison
We evaluated Logistic Regression, Random Forest, and XGBoost (with class imbalance handling).  
XGBoost with `scale_pos_weight=0.5` achieved the best trade-off between precision and recall.

![PR Curve](https://github.com/Hanklin999/images/blob/main/Python_PR_Curve.png)

## Explainability – SHAP
SHAP plots revealed sector and quarter patterns influencing predictions.

![SHAP Sector](https://github.com/Hanklin999/images/blob/main/shap_sector_plot.png)

##  Files
- `earnings_surprise_colab.ipynb`: Full end-to-end pipeline
- `images/`: Visualization assets
- `requirements.txt`: Python package list

##  Appendix – Hyperparameter Tuning
Included sensitivity analysis on `scale_pos_weight` for XGBoost from 0.1 to 1.0
