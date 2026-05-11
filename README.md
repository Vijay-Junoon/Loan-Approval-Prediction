# Loan-Approval-Prediction

## Objective
To study the dataset and conduct proper preprocessing and apply several models and evaluate them independently to find out which model works out the best.

## Dataset
The dataset is titles loan_data.csv. It contains a total of 14000 rows and 14 columns. This encompasses 13 features and 1 target (loan_status)
The features are as follows: 
- person_age
- person_gender
- person_income
- person_emp_exp
- person_home_owndership
- loan_amnt
- loan_int_rate
- loan_percent_income
- cb_person_cred_hist_length
- credit_score
- previous_loan_defaults_on_file
  
## Preprocessing
Things I have considered for effective preprocessing of the above dataset:
- Duplicate values
- Empty / Null values
- Categorical values
- Feature Scaling

### Duplicate Values
There were no duplicate values found in the dataset. 

### Empty/Null values
No Empty or null values were found. So imputation wasn't necessary.

### Categorical values
Out of 13 features, there were 5 categorical values. I chose to OneHotEncode all of these categorical values, to turn them into dummy values.
