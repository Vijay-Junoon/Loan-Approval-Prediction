# Loan Approval Prediction using Machine Learning

## Objective
The objective of this project is to analyze the loan approval dataset, perform effective data preprocessing, train multiple machine learning classification models, and evaluate their performance to determine the most suitable algorithm for predicting loan approval status.

---

## Dataset
The dataset used in this project is **`loan_data.csv`**, consisting of **14,000 rows and 14 columns**, including:

- **13 feature columns**
- **1 target variable (`loan_status`)**

### Features
- `person_age`
- `person_gender`
- `person_education`
- `person_income`
- `person_emp_exp`
- `person_home_ownership`
- `loan_amnt`
- `loan_intent`
- `loan_int_rate`
- `loan_percent_income`
- `cb_person_cred_hist_length`
- `credit_score`
- `previous_loan_defaults_on_file`

### Target Variable
- `loan_status`
  - `1` → Loan Approved
  - `0` → Loan Rejected

---

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

---

## Project Workflow

### 1. Data Analysis
The dataset was analyzed to understand:
- Data types
- Feature distributions
- Categorical and numerical variables
- Correlation between numerical features

### 2. Data Preprocessing

#### Duplicate Value Check
The dataset was checked for duplicate entries.

**Observation:**  
No duplicate values were found.

#### Missing Value Check
The dataset was inspected for null or missing values.

**Observation:**  
No missing values were found; therefore, imputation was not necessary.

#### Categorical Feature Encoding
Out of the 13 features, **5 were categorical**:

- `person_gender`
- `person_education`
- `person_home_ownership`
- `loan_intent`
- `previous_loan_defaults_on_file`

These categorical values were converted into numerical format using **One Hot Encoding**.

#### Feature Scaling
Since numerical features had significantly different ranges, **Standard Scaling** was applied to standardize the dataset.

This preprocessing step was especially important for:
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

Standardization ensures:
- Mean ≈ 0
- Standard Deviation ≈ 1

---

## Machine Learning Models Used

### 1. Random Forest Classifier
**Accuracy:** `92.9%`

Random Forest achieved the best performance among all tested models.

### 2. Support Vector Machine (SVM) Classifier
**Accuracy:** `91.5%`

SVM produced strong performance after feature scaling.

### 3. K-Nearest Neighbors (KNN) Classifier
**Accuracy:** `91.5%`

KNN achieved competitive performance but may be slower for larger datasets.

---

## Model Performance Comparison

| Model | Accuracy |
|--------|----------|
| Random Forest Classifier | 92.9% |
| SVM Classifier | 91.5% |
| KNN Classifier | 91.5% |

---

## Conclusion
Among all the machine learning algorithms evaluated, the **Random Forest Classifier** produced the highest accuracy (**92.9%**) and demonstrated the best performance for predicting loan approval status.

This project demonstrates the importance of:
- Data preprocessing
- Feature encoding
- Feature scaling
- Model comparison and evaluation

in building an effective machine learning classification system.

---
