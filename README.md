# Loan Default Prediction

This project aims to predict whether a loan applicant is likely to default using supervised machine learning techniques. The solution was built using Python and includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation.

---

## Dataset Overview

A synthetic dataset of **500 loan records** was generated for this project. Each record includes:

- `loan_amount`: Total loan amount requested
- `term`: Duration of the loan (in months: 36 or 60)
- `annual_income`: Annual income of the applicant
- `credit_score`: Applicant’s credit score
- `employment_length`: Number of years employed
- `purpose`: Purpose for the loan (e.g., credit card, medical, small business)
- `default`: Binary target (1 = default, 0 = no default)

The dataset is saved as [`loan_data.csv`](./loan_data.csv).

---

## Project Workflow

### 1. Data Cleaning
- Checked for missing values
- Verified data types and formats
- Ensured dataset integrity and structure

### 2. Exploratory Data Analysis (EDA)
- Distribution of numeric features (`credit_score`, `income`, `loan_amount`)
- Class imbalance in the `default` variable
- Relationship between credit score and default behavior

### 3. Feature Engineering
- One-hot encoded the `purpose` column
- Removed unnecessary columns (`loan_id`)
- Created training and testing sets (80/20 split)

### 4. Model Training & Evaluation
Two models were trained and evaluated:
- **Logistic Regression**
- **XGBoost Classifier**

**Evaluation metrics used**:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

---

## Results

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| 50%     |
| XGBoost Classifier | 51%   |

---

## Tools & Technologies

- **Programming**: Python
- **Libraries**: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`
- **Notebook**: Jupyter Notebook
- **File**: [`loan_default_prediction.ipynb`](./loan_default_prediction.ipynb)

---

## Key Takeaways

- XGBoost handled class imbalance and feature interactions better than logistic regression.
- Credit score and income levels were key drivers of loan default probability.
- The model can be enhanced with real-world financial data and more advanced feature engineering (e.g., binning, interaction terms).

---

## 📁 Project Files

- `loan_default_prediction.ipynb`: Full code notebook
- `loan_data.csv`: Dataset
- `README.md`: Project documentation

---

## 📌 Author

**Frederick Kwame Molah**  
Email: frederickmolah@gmail.com  
[LinkedIn](https://www.linkedin.com/in/frederick-molah-b36a64159/)
