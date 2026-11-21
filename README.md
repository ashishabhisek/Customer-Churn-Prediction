# Customer Churn Prediction App

An end-to-end Machine Learning application that predicts customer churn probability using customer demographics, service usage, account information, and billing data.

The project focuses on building a complete ML pipeline, from data analysis and preprocessing to model development, explainability, and deployment.

## 1. Dataset

**Dataset:** Telco Customer Churn (Kaggle)  
**Link:** https://www.kaggle.com/datasets/blastchar/telco-customer-churn

- 7,043 customer records
- 21 features
- Target Variable: `Churn`

The dataset includes customer demographics, subscription details, internet services, contract types, and billing information.

## 2. Tech Stack

- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, XGBoost
- **Visualization:** Matplotlib
- **Explainable AI:** SHAP
- **Deployment:** Streamlit
- **Model Saving:** Joblib

## 3. Machine Learning Workflow

- **EDA:** Analyzed customer behavior, churn distribution, and feature relationships.
- **Preprocessing:** Missing value imputation, standard scaling, and one-hot encoding using `ColumnTransformer`.
- **Model Training:** Trained and compared Logistic Regression, Random Forest, and XGBoost.
- **Class Imbalance:** Handled using appropriate balancing techniques and class weights.
- **Threshold Optimization:** Evaluated different classification thresholds to balance precision and recall.
- **Explainability:** Used SHAP to understand feature importance and individual predictions.

## 4. Model Performance

| Model | ROC-AUC | F1 Score | Precision | Recall |
|---|---:|---:|---:|---:|
| Logistic Regression | 0.86 | 0.64 | 0.52 | 0.84 |
| Random Forest | 0.85 | 0.65 | 0.56 | 0.78 |
| XGBoost | 0.85 | 0.63 | 0.55 | 0.75 |

## 5. Key Insights

- Customers with month-to-month contracts have higher churn rates.
- Lower customer tenure is associated with increased churn.
- Higher monthly charges can contribute to churn.
- Customers without additional services like Online Security and Tech Support show higher churn tendencies.

## 6. Business Recommendations

- Encourage long-term subscriptions through discounts.
- Offer bundled services to improve customer retention.
- Provide personalized offers to high-risk customers.
- Focus on early engagement with new customers.

## 7. Deployment

The application is deployed using **Streamlit**, allowing users to:

- Enter customer information.
- Get real-time churn probability predictions.
- Identify potential churn risks.
- Understand predictions through SHAP explanations.

## 8. Conclusion

This project demonstrates how Machine Learning and Explainable AI can help businesses identify potential customer churn, understand customer behavior, and develop data-driven retention strategies.

**Goal: Predict customer churn and turn insights into better retention decisions.**
