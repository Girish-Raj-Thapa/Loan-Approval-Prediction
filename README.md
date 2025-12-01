
# Loan Approval Prediction
A Machine Learning Classification Project Using Kaggle Dataset

This project builds a supervised machine learning model to predict whether a loan application will be Approved or Rejected based on financial, credit, and demographic features of applicants. All analysis, modeling, and prediction steps are implemented in a single Jupyter Notebook.

## Project Files
| File | Description |
|------|-------------|
| loan_approval_dataset.csv | Kaggle dataset used for training and evaluation. |
| loan_approval_prediction.ipynb | Jupyter Notebook containing the entire ML workflow (EDA → Preprocessing → Modeling → Predictions). |
| loan_approval_predictions.csv | Model output file containing predicted approval decisions. |

## Dataset Description
The dataset includes 4,269 loan applicant records with 13 attributes (10 numerical and 3 categorical). No missing values are present.

### Feature Summary
- loan_id — Unique identifier  
- no_of_dependents — Number of dependents  
- education — Graduate / Not Graduate  
- self_employed — Yes / No  
- income_annum — Annual income  
- loan_amount — Requested amount  
- loan_term — Duration in months  
- cibil_score — Credit score  
- residential_assets_value — Residential property value  
- commercial_assets_value — Commercial property value  
- luxury_assets_value — Luxury assets owned  
- bank_asset_value — Bank assets  
- loan_status — Target variable (Approved / Rejected)

## Workflow Overview
All steps are executed inside loan_approval_prediction.ipynb:

1. Load & inspect dataset  
2. Exploratory Data Analysis (EDA)  
3. Data preprocessing  
4. Model training (Logistic Regression, Decision Tree, Random Forest, SVM, KNN)  
5. Model evaluation (Accuracy, Precision, Recall, F1-score, ROC-AUC)  

## Best Model: Random Forest
- Test Accuracy: 96.5%  
- Precision: 92.2%  
- Recall: 99.1%  
- F1-score: 95.5%  
- ROC-AUC: 99.2%

## Output File
`loan_approval_predictions.csv` contains:
- Loan IDs  
- Predicted status  
- Probability scores  

## How to Run
```
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook loan_approval_prediction.ipynb
```

## Future Enhancements
- Hyperparameter tuning  
- Deployment with Flask/FastAPI  
- Streamlit dashboard  
- SHAP explainability  

## Author
Girish Raj Thapa
