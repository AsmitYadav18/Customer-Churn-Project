# Customer Churn Prediction – Credit Card Customers

**Author:** Asmit Yadav  
**Domain:** Banking / Credit Card Analytics  
**Skills Demonstrated:** Python, EDA, ML Models, Feature Engineering, Model Evaluation

---

## 🚀 Project Overview
Predict **customer churn** for credit card users using **Machine Learning**.  
Customer churn occurs when a customer stops using the service. Predicting churn helps **retain customers and increase revenue**.

**Data Cleaning Highlight:**  
We removed the **Naive Bayes probability columns** (derived features) to **prevent data leakage**, ensuring the model only learns from realistic, available features.

---

## 🗂 Dataset
- **Rows:** 10,127  
- **Columns:** 23 (including `Attrition_Flag`)  
- **Source:** Credit Card Customer Data  
- **Key Features:**  
  - Demographics: Customer_Age, Gender, Income_Category  
  - Card/Relationship: Card_Category, Months_on_book  
  - Credit Usage: Credit_Limit, Total_Revolving_Bal  
  - Transactions: Total_Trans_Amt, Total_Trans_Ct  
  - Engagement: Months_Inactive_12_mon, Contacts_Count_12_mon  

---

## 🔎 EDA Insights
- High inactivity → higher churn  
- Premium cardholders more likely to churn  
- Customers with more transactions are less likely to churn  
- Avg_Open_To_Buy correlates with churn patterns  

---

## 🧠 Models Trained

| Model | Accuracy | F1 Score (Churn) |
|-------|---------|----------------|
| Random Forest | 95% | 82% |
| Decision Tree | 94% | 79% |
| AdaBoost | 94% | 80% |
| SVM | 92% | 68% |
| **XGBoost** | **97%** | **91%** |
| Logistic Regression | 90% | 65% |

**Best Model:** XGBoost  

---

## 📂 Project Structure
customer-churn-project/
│
├── data/
│ └── BankChurners.csv
├── Project.ipynb
└── README.md
