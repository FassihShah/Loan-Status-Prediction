# Loan Status Prediction using Machine Learning

This project predicts whether a loan application will be **approved or not** based on various applicant details using a **Support Vector Machine (SVM)** classifier.

---

## Files in this Repository

- `Loan_Status_Prediction.ipynb` – Jupyter Notebook with the complete ML pipeline
- `README.md` – Project documentation

---

## Dataset Description

The dataset contains information about applicants such as gender, income, education, employment, credit history, etc., along with the loan status (approved or not).

| Feature | Description |
|---------|-------------|
| Gender | Male/Female |
| Married | Yes/No |
| Education | Graduate/Not Graduate |
| Self_Employed | Yes/No |
| ApplicantIncome | Income of applicant |
| LoanAmount | Loan amount |
| Loan_Status | Y/N (Target Variable) |

---

## Steps Performed

1. **Data Loading**  
   - Loaded the dataset from CSV

2. **Data Cleaning**  
   - Handled missing values by dropping them
   - Replaced categorical values with numerical labels

3. **Label Encoding**  
   - Converted 'Y' to `1` and 'N' to `0` in `Loan_Status`

4. **Feature Selection**  
   - Dropped `Loan_ID` and target label for `X`

5. **Train-Test Split**  
   - Split data with `test_size=0.1` and `stratify=Y`

6. **Model Training**  
   - Used **Support Vector Machine** with linear kernel

7. **Evaluation**  
   - Calculated accuracy for both training and testing sets

---

## Results

- **Accuracy on Training Data**: 80%  
- **Accuracy on Test Data**: 83.4%

---
