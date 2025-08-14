# Credit Risk Prediction

## 📌 Objective
Predict whether a loan applicant is likely to **default on a loan** based on demographic and financial features.

This project uses **Logistic Regression** and **Decision Tree Classifier** to model the likelihood of loan approval/default, with a focus on:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Model training and evaluation
- Performance comparison between classifiers

---

## 📂 Dataset
**Source:** [Loan Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/ninzaami/loan-predication)  

The dataset contains applicant demographic information, loan details, and the loan approval status.

**Key Columns:**
- `Gender` – Applicant gender
- `Married` – Marital status
- `Dependents` – Number of dependents
- `Education` – Education level
- `Self_Employed` – Self-employment status
- `ApplicantIncome` – Monthly income of applicant
- `CoapplicantIncome` – Monthly income of co-applicant
- `LoanAmount` – Loan amount in thousands
- `Loan_Amount_Term` – Loan term in months
- `Credit_History` – Credit history (1 = good, 0 = bad)
- `Loan_Status` – Target variable (Y = approved, N = not approved)

---

## 👉 Steps Performed

### **1. Data Cleaning**
- Handled missing values:
  - Categorical → filled with **mode**
  - Numerical → filled with **median**
- Checked for and confirmed **no missing values** after cleaning.

### **2. Exploratory Data Analysis (EDA)**
- Visualized:
  - Distribution of Loan Amount
  - Loan Status by Education Level
  - Applicant & Coapplicant Income distributions
  - Scatter plot: Income vs Loan Amount (colored by Loan Status)
- Generated correlation heatmap for numerical features

### **3. Model Training**
- **Logistic Regression**
- **Decision Tree Classifier**

### **4. Model Evaluation**
- Accuracy score
- Confusion Matrix
- Classification Report (precision, recall, F1-score)
- ROC Curve & AUC score

---

## 📊 Results

| Model                  | Accuracy | AUC  | Precision (Class 1) | Recall (Class 1) | F1-score (Class 1) |
|------------------------|----------|------|---------------------|------------------|--------------------|
| Logistic Regression    | 0.789    | 0.75 | 0.76                | 0.99             | 0.86               |
| Decision Tree          | 0.772    | 0.72 | 0.75                | 0.96             | 0.85               |
