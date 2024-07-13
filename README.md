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

The dataset used 255,347 rows from 18 variables, but only uses a few variables that are relevant in influencing/evaluating loan default. The data is a collection of information that includes demographic, financial, and loan information. The data consists of :

15 predictors/potential characteristics - 1 response/target variable

### Predictor :
1. Age: The age of the borrower.
2. Income: Annual income of the borrower.
3. LoanAmount:  The total amount of money borrowed.
4. MonthsEmployed: The number of months the borrower has been employed.
5. NumCreditLines: The number of credit lines the borrower has open.
6. InterestRate: The interest rate of the loan.
7. LoanTerm: The term or duration of the loan in months
8. DTIRatio: Debt-to-Income ratio, calculated as total monthly debt payments divided by gross monthly income
9. Education: The educational level of the borrower (e.g., High School, Bachelor's, Master's).
10. EmploymentType: The type of employment the borrower has (e.g., Salaried, Self-employed, Unemployed).
11. MaritalStatus: The marital status of the borrower (e.g., Single, Married, Divorced).
12. HasMortgage: Indicates whether the borrower has a mortgage (1 for yes, 0 for no).
13. HasDependents: Indicates whether the borrower has dependents (1 for yes, 0 for no).
14. LoanPurpose: The purpose of the loan (e.g., Education, Car Purchase, Home Improvement).
15. HasCoSigner: : Indicates whether the loan has a co-signer (1 for yes, 0 for no).

### Target
1. Default: The target variable indicating whether the loan defaulted (1 for default, 0 for no default).
