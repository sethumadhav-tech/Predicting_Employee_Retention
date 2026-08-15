# Predicting Employee Retention

## 📌 Project Overview

Employee attrition is a major business challenge because losing experienced employees can increase recruitment costs, reduce productivity, and affect team performance.

This project analyzes employee data from a mid-sized technology company to understand the key factors associated with employee attrition and builds a **Logistic Regression model** to predict whether an employee is likely to stay or leave.

The project covers:

- Data understanding
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature encoding
- Feature scaling
- Recursive Feature Elimination (RFE)
- Logistic Regression
- Multicollinearity analysis using VIF
- Classification evaluation
- Cutoff analysis
- Business insights and HR recommendations

---

## 🎯 Business Problem

A mid-sized technology company is facing challenges in retaining employees.

The objective is to:

1. Identify the factors associated with employee attrition.
2. Understand employee behavior and risk patterns.
3. Build a predictive model to identify employees who may leave.
4. Translate the analysis into actionable HR strategies.

The ultimate goal is to help HR teams make **data-driven employee-retention decisions**.

---

## 📊 Key Business Insights

### 1. Employee Satisfaction

Employees with lower satisfaction levels are more likely to leave.

**Business implication:** Regular employee feedback and engagement initiatives can help identify dissatisfaction early.

### 2. Workload

High average monthly working hours and project counts are associated with higher attrition.

**Business implication:** Workloads and project assignments should be monitored to reduce employee burnout.

### 3. Salary

Employees with lower salary levels show substantially higher attrition.

**Business implication:** Compensation benchmarking and competitive pay can help improve employee retention.

### 4. Career Growth

Limited promotion opportunities and shorter tenure are associated with higher attrition.

**Business implication:** Clear career-development paths and recognition programs can improve employee retention.

---

## 🔎 Analysis Approach

### 1. Data Understanding

The employee dataset was analyzed to understand variables related to:

- Employee satisfaction
- Number of projects
- Average monthly hours
- Salary
- Department
- Tenure
- Promotion
- Employee attrition

### 2. Data Cleaning & Preprocessing

The project includes:

- Missing-value checks
- Data-type checks
- Categorical-variable encoding
- One-hot encoding
- Target-variable conversion
- Removal of redundant encoded variables
- Feature scaling

### 3. Exploratory Data Analysis

The analysis investigates relationships between employee attrition and:

- Satisfaction level
- Number of projects
- Average monthly hours
- Salary
- Other employee-related variables

Correlation analysis and visualizations are also used to understand relationships among features.

### 4. Feature Selection

**Recursive Feature Elimination (RFE)** is used with Logistic Regression to select important features.

### 5. Logistic Regression

A Logistic Regression model is developed to predict employee retention/attrition.

The model is also analyzed using statistical measures such as:

- Coefficients
- p-values
- Statistical significance

### 6. Multicollinearity Analysis

**Variance Inflation Factor (VIF)** is used to identify potential multicollinearity among predictors.

### 7. Model Evaluation

The model evaluation includes:

- Accuracy
- Confusion Matrix
- Sensitivity
- Specificity
- Precision
- Recall
- ROC analysis
- Precision-Recall analysis
- Probability cutoff analysis

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression was selected because the target variable represents a binary employee-retention outcome.

The model estimates the probability of an employee belonging to the target class based on employee-related attributes.

---

## ⚠️ Model Evaluation & Limitation

The current notebook contains the complete modeling workflow, but the saved model outputs show a **degenerate prediction result** where the model predicts only one class.

The recorded validation confusion matrix is:

```text
[[2868,    0],
 [2953,    0]]
