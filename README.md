# ChurnGuard AI

A machine-learning app that predicts which telecom customers are likely to cancel, explains why, and estimates whether a retention offer is worth the cost.

# What it does
- Trains and compares Logistic Regression, Random Forest and XGBoost on the public IBM Telco churn dataset (7,043 customers)
- Picks the decision threshold that maximizes dollar benefit, not accuracy
- Explains each prediction with SHAP
- Provides a Streamlit app for scoring one customer, scoring a whole list, and testing business assumptions

# Tech: Python, scikit-learn, XGBoost, SHAP, Streamlit
