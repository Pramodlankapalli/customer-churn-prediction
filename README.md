# Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn using a telecom dataset.  
The objective is to identify customers who are likely to leave the company so that proactive retention strategies can be applied.

Customer churn prediction is important because retaining existing customers is more cost-effective than acquiring new ones.

---

## Dataset

- Source: Kaggle (Telco Customer Churn Dataset)
- Total Records: 7000+ customers
- Target Variable: `Churn` (Yes / No)

The dataset contains customer demographic details, subscribed services, contract type, tenure, billing information, and payment methods.

---

## Project Workflow

### 1. Data Loading & Understanding
- Loaded dataset using pandas
- Checked data types and missing values
- Understood feature distributions

### 2. Data Cleaning & Preprocessing
- Converted categorical features into numerical format
- Handled data inconsistencies
- Verified no missing values remained

### 3. Exploratory Data Analysis (EDA)
- Analyzed overall churn distribution
- Compared churn rate across contract types
- Observed higher churn in month-to-month contracts
- Found that customers with higher monthly charges tend to churn more

### 4. Feature Engineering
- Encoded categorical variables
- Split data into training and testing sets

### 5. Model Building & Evaluation

The following models were implemented and compared:

- Logistic Regression (baseline model)
- Random Forest Classifier
- XGBoost Classifier

Model performance was evaluated using Accuracy and Recall.

Since identifying churn customers is more important than just achieving high accuracy, recall was given higher importance during evaluation.

---

## Model Performance

- Logistic Regression Accuracy: ~78%
- Random Forest Accuracy: ~79%
- Recall improved to ~0.70 after tuning

After comparing all models and considering business impact, **Random Forest was selected as the final model** because it provided a better balance between accuracy and recall.

---

## Key Insights

- Customers with month-to-month contracts are more likely to churn.
- Longer tenure customers are less likely to leave.
- Higher monthly charges slightly increase churn probability.

---

## Conclusion

In this project, multiple machine learning models were implemented and compared to predict customer churn. Logistic Regression, Random Forest, and XGBoost were used for performance comparison.

After evaluating model metrics and considering business impact, Random Forest was selected as the final model.

The project demonstrates a complete end-to-end machine learning workflow, including preprocessing, model building, evaluation, and comparison of multiple models.

---

## Future Improvements

- Perform advanced hyperparameter tuning to further improve model performance.
- Apply imbalance handling techniques such as SMOTE to balance precision and recall.
- Improve feature engineering to capture more meaningful patterns from data.
- Deploy the model using Streamlit to make it more user-friendly and practical.

---

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## Author

Pramod Lankapalli  
Aspiring Data Scientist
