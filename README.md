# 🏦 Bank Loan Risk Analysis (R + Power BI)

## 📘 Project Overview
This project aims to predict **loan applicant risk** (High vs. Low) using applicant data such as **income, age, credit score, loan amount**, and other financial indicators.  
We build a **classification model in R** and then visualize insights through an **interactive Power BI dashboard**.

---

## 🎯 Objectives
- Classify loan applicants into **High Risk** or **Low Risk** categories.  
- Identify **key features** affecting loan default.  
- Build a **machine learning model** to predict loan risk.  
- Create a **Power BI dashboard** for visual analytics.

---

## 🧩 Dataset
**Source:** [Bank Loan Data – Kaggle](https://www.kaggle.com/datasets/udaymalviya/bank-loan-data)

**Description:**
The dataset contains details about loan applicants, including:
- Age  
- Income  
- Loan Amount  
- Credit Score  
- Employment Type  
- Loan Purpose  
- Default (Target Variable: 1 = High Risk, 0 = Low Risk)

**Rows:** 45,000+  
**Columns:** 8–10 (depending on preprocessing)

---

## 🧠 Tech Stack
| Tool | Purpose |
|------|----------|
| **R** | Data cleaning, preprocessing, modeling |
| **Power BI** | Visualization and dashboard building |
| **Libraries Used (R)** | dplyr, caret, ggplot2, randomForest, e1071, ROCR |

---

## ⚙️ Steps Followed

### **Step 1: Data Loading & Exploration**
- Imported CSV dataset using `readr`  
- Checked structure, summary statistics, and missing values  
- Visualized distributions for **age, income, and credit score**

### **Step 2: Data Cleaning & Feature Engineering**
- Replaced missing numeric values with median  
- Replaced missing categorical values with mode  
- Converted text columns to factors  
- Scaled numeric features using `caret`  
- Created new feature: `debt_to_income_ratio`

### **Step 3: Model Building & Evaluation**
Built and compared three models:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**

Evaluated with **accuracy** and **confusion matrix**.  
The **Random Forest** model achieved the highest performance.

### **Step 4: Power BI Dashboard**
Exported processed data and results to Power BI:
- `loan_cleaned_data.csv`  
- `model_accuracy.csv`  
- `feature_importance.csv`

**Dashboard Pages:**
1. **Overview:** Applicant demographics and risk distribution  
2. **Risk Analysis:** Income vs credit score patterns  
3. **Model Performance:** Accuracy comparison & feature importance  
4. **Interactive Filters:** Explore applicants by age, income, or risk category  

---

## 📊 Key Insights
- Applicants with **low credit scores** and **high debt-to-income ratios** are more likely to default.  
- **Income** and **credit score** are the strongest predictors of risk.  
- **Random Forest** achieved the highest accuracy (~90%+).  
- Majority of applicants fall in **Low Risk** category.

---