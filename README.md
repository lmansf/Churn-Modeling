# Churn-Modeling
Using Ensemble Learning to achieve high accuracy Churn modeling
## Dataset
The dataset used is the Customer Churn dataset from Kaggle found here: https://www.kaggle.com/datasets/barun2104/telecom-churn/data
- The dataset already contains past churn, removing any need to estimate or label that, and enabling supervised learning methods
- The dataset already contains important features, so there's no need to do feature engineering in this scenario.
## Handling the Dataset
- The dataset is split into a validation and training set based on the "AccountWeeks" column. accounts with less than 97 Account Weeks were used for validation, and those with 97 or more account weeks were used as historical training data. The split is about 1500 records for each.

## Models
The models tested include:
- XGBoost
- Naive Bayes Regression
- Random Forest Regression
- Kernel Support Vector Machine
- Ensemble Learning
## Performance
- Using a strict ensemble configuration (unanimous only), the model predicts churn on the validation data with 93% accuracy, making it viable in real world business use-cases.
