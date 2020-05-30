# LendingClub_Kaggle
Dataset of approx. 0.4 million loans. Predicting loan repay status
LendingClub DataSet obtained from Kaggle: https://www.kaggle.com/wordsforthewise/lending-club
Given the data on loans previously taken form LendingClub, the aim is to create a model that can predict wether or not a new borrower will pay back loan

## PART A. EXPLORATORY DATA ANANLYSIS
Following inference drawn:
- dataset is somewhat unbalanced
- Installment is highly correlated with loan amount
- Unpaid loans corresponds to slightly higher loan amount
- The default rate is too high in F and G graded loans
- Higher the interest rate, more is the chance of default
![alt text](https://github.com/ravigupta5/LendingClub_Kaggle/blob/master/grades.PNG?raw=true)

## PART B. DATA PREPROCESSING
1. HANDLING MISSING DATA
    - emp_title
    - emp_length
    - title column
    - mort_acc feature
    - revol_util
    - pub_rec_bankruptcies
    
2. HANDLING CATEGORICAL DATA
    - term
    - grade
    - sub_grade
    - verification_status, application_type,initial_list_status,purpose
    - home_ownership
    - address
    - issue_id
    - earliest_cr_line

## PART C. CREATING MODEL
Applied Random Forest Model to get f1 score of 0.93 and 0.63 for loan_repaid and not_paid categories respectively
