# Revolut Fraud Detection

StrataScratch data science challenge based on fictional Revolut banking data.

## Objective
Build a machine learning model to identify fraudulent users from fictional banking data.

## Data
- `users.csv` — user profiles including KYC status, country, and account details
- `transactions.csv` — transaction history including amount, type, and currency

## Approach
1. **EDA** — explored fraud patterns across KYC status, transaction type, and user behavior
2. **Feature Engineering** — built user-level features from both datasets based on fraud behavior hypotheses
3. **Modelling** — compared Logistic Regression, Random Forest, and Gradient Boosting
4. **Hyperparameter Tuning** — used GridSearchCV with recall as the optimization metric

## Key Findings
- PENDING KYC users have the highest fraud rate at 21%
- Fraudsters overindex on ATM and TOPUP transactions
- Failed sign in attempts are twice as high among fraudsters
- Random Forest selected as final model — best balance between recall and precision

## Tech Stack
Python, pandas, scikit-learn, matplotlib
