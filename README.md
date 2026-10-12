# ChurnGuard AI

A machine-learning app that predicts which telecom customers are likely to cancel, explains why, and estimates whether a retention offer is worth the cost.

# What it does
- Trains and compares Logistic Regression, Random Forest and XGBoost on the public IBM Telco churn dataset (7,043 customers)
- Picks the decision threshold that maximizes dollar benefit, not accuracy
- Explains each prediction with SHAP
- Provides a Streamlit app for scoring one customer, scoring a whole list, and testing business assumptions

# Tech: Python, scikit-learn, XGBoost, SHAP, Streamlit

# Instructions to use the application: 
python -m venv .venv
.venv\Scripts\activate          # Mac/Linux: source .venv/bin/activate
pip install -r requirements.txt
python train.py                 # trains the models and saves reports
python -m pytest -q             # runs the tests
streamlit run app.py            # opens the app at http://localhost:8501
```

## Project structure
- `app.py`: Streamlit app
- `train.py`: training, evaluation and SHAP
- `src/`: data, model, ROI and explainability code
- `docs/`: process guide, Q&A prep and presentation script
- `reports/`: generated plots and metrics

