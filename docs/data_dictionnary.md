# 📚 Data Dictionary

This document describes the fields available in the two datasets used in this fraud detection project:
- `loan_applications.csv`: information about loan applications
- `transaction.csv`: information about customer financial transactions

---

## 📂 loan_applications.csv

| Column                        | Type     | Description                                                                 |
|------------------------------|----------|-----------------------------------------------------------------------------|
| application_id               | object   | Unique ID of the loan application                                           |
| customer_id                  | object   | Unique identifier of the customer                                           |
| application_date             | object   | Date of the loan application                                                |
| loan_type                    | object   | Type of loan requested (Home, Personal, Education, etc.)                   |
| loan_amount_requested        | float64  | Amount requested in the loan application                                   |
| loan_tenure_months           | int64    | Duration of the loan in months                                              |
| interest_rate_offered        | float64  | Interest rate offered for the loan                                          |
| purpose_of_loan              | object   | Purpose or reason behind the loan request                                  |
| employment_status            | object   | Employment status of the applicant (e.g. Employed, Self-employed, etc.)    |
| monthly_income               | float64  | Monthly income of the applicant                                             |
| cibil_score                  | int64    | Credit score of the applicant                                               |
| existing_emis_monthly        | float64  | Monthly payment amount of existing loans (EMIs)                            |
| debt_to_income_ratio         | float64  | Ratio of total debt to monthly income                                      |
| property_ownership_status    | object   | Indicates whether the applicant owns, rents, or leases a property          |
| residential_address          | object   | Residential address of the applicant                                        |
| applicant_age                | int64    | Age of the loan applicant                                                   |
| gender                       | object   | Gender of the applicant                                                     |
| number_of_dependents         | int64    | Number of people financially dependent on the applicant                    |
| loan_status                  | object   | Status of the loan application (e.g. Approved, Rejected)                   |
| fraud_flag                   | int64    | Indicates if the loan application was fraudulent (1 = Fraud, 0 = Legit)    |
| fraud_type                   | object   | Type of fraud detected (if any); mostly null                               |

---

## 📂 transaction.csv

| Column                         | Type     | Description                                                                 |
|--------------------------------|----------|-----------------------------------------------------------------------------|
| transaction_id                 | object   | Unique identifier of the transaction                                        |
| customer_id                    | object   | Identifier of the customer who made the transaction                         |
| transaction_date               | object   | Date of the transaction                                                     |
| transaction_type               | object   | Nature of the transaction (e.g. POS, ATM, Online, Loan Disbursement)       |
| transaction_amount             | float64  | Amount involved in the transaction                                          |
| merchant_category              | object   | Category of the merchant (e.g. Electronics, Travel, Food)                  |
| merchant_name                  | object   | Name of the merchant                                                        |
| transaction_location           | object   | Location where the transaction occurred                                     |
| account_balance_after_transaction | float64  | Balance in the account after the transaction                                |
| is_international_transaction   | int64    | 1 = Transaction occurred abroad, 0 = Domestic transaction                   |
| device_used                    | object   | Device used to perform the transaction (e.g. Mobile, POS, Desktop)         |
| ip_address                     | object   | IP address used for the transaction                                         |
| transaction_status             | object   | Status of the transaction (e.g. Success, Failed, Reversed)                 |
| transaction_source_destination| object   | Source and destination of transaction (e.g. Customer to Merchant)          |
| transaction_notes              | object   | Free-text notes about the transaction (if any)                              |
| fraud_flag                     | int64    | Indicates if the transaction was fraudulent (1 = Fraud, 0 = Legit)         |
