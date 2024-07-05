# **Loan Default Project**

![workflow status](https://github.com/uyunmubarak/loan-default-project/actions/workflows/builder.yml/badge.svg)

Steps:
+ Select **Use this template** > **Create a new repository**. This menu is in the top right corner of this repository.
+ Edit `setup.py` and define your the project repository.
+ Rename `src/MLProject` to your project name.
+ Create virtual environment

    ```bash
    virtualenv .venv -p /usr/bin/python3.10
    ```
  **Note:** You can use any Python version, as long the Python packages in `requirements.txt` are supported. Because of the Python packages in `requirements.txt` were declared without describe the version.
+ Activate the virtual environment

    ```bash
    source .venv/bin/activate
    ```

+ Install package.

    ```bash
    pip install -r requirements.txt
    ```

+ enable the environment variables.

    ```bash
    cp .env.example .env
    ```

## Loan Default Dataset Description
### Overview

The Loan Default dataset provides comprehensive information about borrowers and their loans. The dataset is used to analyze and predict the likelihood of a borrower defaulting on a loan. It contains a mix of numerical and categorical features that describe both the borrower's characteristics and the details of their loans.

### Columns :
1. LoanID : Unique identifier for each loan.
2. Age: The age of the borrower.
3. Income: Annual income of the borrower.
4. LoanAmount:  The total amount of money borrowed.
5. MonthsEmployed: The number of months the borrower has been employed.
6. NumCreditLines: The number of credit lines the borrower has open.
7. InterestRate: The interest rate of the loan.
8. LoanTerm: The term or duration of the loan in months
9. DTIRatio: Debt-to-Income ratio, calculated as total monthly debt payments divided by gross monthly income
10. Education: The educational level of the borrower (e.g., High School, Bachelor's, Master's).
11. EmploymentType: The type of employment the borrower has (e.g., Salaried, Self-employed, Unemployed).
12. MaritalStatus: The marital status of the borrower (e.g., Single, Married, Divorced).
13. HasMortgage: Indicates whether the borrower has a mortgage (1 for yes, 0 for no).
14. HasDependents: Indicates whether the borrower has dependents (1 for yes, 0 for no).
15. LoanPurpose: The purpose of the loan (e.g., Education, Car Purchase, Home Improvement).
16. HasCoSigner: : Indicates whether the loan has a co-signer (1 for yes, 0 for no).
17. Default: The target variable indicating whether the loan defaulted (1 for default, 0 for no default).

### Potential Applications
Credit Risk Assessment: Helping financial institutions assess the risk associated with loan applications.
Customer Segmentation: Identifying patterns among borrowers who are more likely to default.
Policy Formulation: Assisting in the formulation of policies to mitigate default risks.