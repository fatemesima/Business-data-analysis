# Telecom Churn Prediction (Stacking Ensemble + SHAP)


**Project goal:** Predict customer churn for a subscription telecom service and deliver business-ready insights (KPI, drivers of churn, recommendations).


## Contents
- `notebooks/churn_modeling.ipynb`: Clean notebook with EDA, KPI, modeling (baseline, XGBoost, LightGBM, stacking), evaluation and SHAP analysis.
- `reports/images/shap_summary.png`: SHAP summary plot (only image included per request).
- `requirements.txt`: Python packages used.


## KPIs computed
- Churn Rate
- ARPU (Average Revenue Per User)
- Average Tenure
- Simple Estimated LTV


## Modeling
- Baseline: Logistic Regression
- Tree models: Random Forest, XGBoost, LightGBM
- Ensemble: StackingClassifier with Logistic / Ridge meta-model


## Explainability
- SHAP is used to explain the XGBoost base learner (SHAP summary plot included in `images/Capture3.JPG`).


## How to run (quick)
1. Create a new GitHub repo and clone it locally or open a Colab notebook.
2. Copy notebook code into `notebooks/churn_modeling.ipynb` (sections are provided in the notebook).
3. Place the SHAP image at `reports/images/shap_summary.png`.
4. Install requirements: `pip install -r requirements.txt`.
5. Run the notebook cell-by-cell. Use `joblib` to save final model artifacts if needed.


