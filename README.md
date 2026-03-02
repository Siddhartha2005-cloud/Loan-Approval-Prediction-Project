# Loan-Approval-Prediction-Project
This project aims to analyze loan application data to identify patterns and build machine learning models that predict loan approval status based on applicant demographics and financial information.
## Project Structure

The project is divided into three main notebooks:

1. **`1_EDA.ipynb`**: Focused on data cleaning and exploratory data analysis to understand the dataset.
2. **`2_loan_approval_using_decision_tree.ipynb`**: Implements a Decision Tree classifier to predict loan status.
3. **`3_loan_approval_using_logictic_regression.ipynb`**: Implements a Logistic Regression model for the same prediction task.

## Dataset Overview

The analysis uses a dataset of 45,000 loan applications with the following characteristics:

* **No Missing Values**: The dataset is complete with 0 missing values across all 14 columns.
* **No Duplicates**: There are no duplicated rows in the data.
* **Key Features**: Includes applicant age, gender, education, income, employment experience, home ownership, loan amount, intent, interest rate, and credit score.

## Key Insights from EDA

* **Education Trends**: Applicants with a Bachelor's degree apply for loans the most frequently, while those with a Doctorate apply the least.
* **Approval Rates**:
* Bachelors have the highest number of both accepted and rejected loan applications.
* Masters degree holders have the highest overall loan acceptance rate.


* **Demographics**: The average applicant age is approximately 27.8 years.

## Model Performance

Two models were evaluated for their ability to predict loan approval ("Yes" or "No"):

### Decision Tree Model

* **Configuration**: Trained using the `entropy` criterion and a `max_depth` of 11.
* **Accuracy**: 92%.
* **Performance (Approved Class)**: Achieved a precision of 0.88 and a recall of 0.74, resulting in an F1-score of 0.80.

### Logistic Regression Model

* **Configuration**: Trained using default hyperparameters.
* **Accuracy**: 90%.
* **Performance (Approved Class)**: Achieved a precision of 0.78 and a recall of 0.78, resulting in an F1-score of 0.78.

## Conclusion

The **Decision Tree** model outperformed Logistic Regression in terms of overall accuracy (92% vs 90%) and precision for approved loans. However, the **Logistic Regression** model provided a more balanced precision and recall (both 0.78) for the approved class.
