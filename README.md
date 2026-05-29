# Credit Risk Classifier

## What it does
A machine learning model that predicts whether a loan applicant 
will default or not, using the German Credit dataset.

## Models 
- Logistic Regression (AUC: 0.75)
- Random Forest (AUC: 0.77)

## Findings
- Credit amount, age, and duration were the strongest predictors of default
- Missing checking account information was itself a signal of higher risk
- Random Forest marginally outperformed Logistic Regression but Logistic 
  Regression is preferred for its interpretability in a risk setting

## Limits
- Dataset is only 1000 rows which limits model accuracy
- Class imbalance 700 good, 300 bad affects recall on defaults
- With more data SMOTE to add more 'bad' data sets or threshold tuning

## How to run
1. Clone the repo
2. Create a virtual environment: `python3 -m venv venv`
3. Activate it: `source venv/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`
5. Open `notebooks/credit_risk.ipynb` and run all cells