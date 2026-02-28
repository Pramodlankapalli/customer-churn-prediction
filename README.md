# Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn using a telecom dataset. 
The main objective is to identify customers who are likely to leave the company so that appropriate retention strategies can be applied.

Customer churn prediction is important because acquiring a new customer is more expensive than retaining an existing one.

---

## Dataset

- Source: Kaggle (Telco Customer Churn Dataset)
- Total records: 7000+ customers
- Target variable: `Churn` (Yes / No)

The dataset includes customer demographics, services subscribed, contract type, tenure, payment method, and billing details.

---

## Project Workflow

### 1. Data Loading and Inspection
- Loaded the dataset using pandas
- Checked data types and missing values
- Understood feature distribution

### 2. Data Cleaning
- Converted categorical columns into numerical format
- Removed unnecessary columns
- Verified no null values remained

### 3. Exploratory Data Analysis (EDA)
- Analyzed churn distribution
- Compared churn with contract type and tenure
- Observed that month-to-month contract customers churn more
- Found that higher monthly charges increase churn probability

### 4. Feature Engineering
- Encoded categorical variables
- Split data into training and testing sets

### 5. Model Building
Built and evaluated multiple models:

- Logistic Regression (baseline model)
- Random Forest Classifier

Model performance was compared using accuracy and recall.

---

## Model Performance

- Logistic Regression Accuracy: ~78%
- Random Forest Accuracy: ~79%
- Recall improved to ~0.70 after tuning

Improving recall was important because correctly identifying churn customers is more critical than just achieving high accuracy.

---

## Key Insights

- Customers with month-to-month contracts are more likely to churn
- Customers with longer tenure are less likely to leave
- Higher monthly charges slightly increase churn probability

---

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Future Improvements

- Hyperparameter tuning using GridSearchCV
- Trying advanced models like XGBoost
- Deploying the model using Streamlit
- Adding business cost-based evaluation

---

## Author

Pramod Lankapalli  
Aspiring Data Scientist
