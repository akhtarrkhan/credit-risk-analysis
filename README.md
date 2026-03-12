# Credit Risk Analysis using Python

## Overview

This project explores a consumer loan dataset to understand the factors associated with loan default. Using Python and data analysis techniques, the project investigates borrower characteristics, loan attributes and financial indicators that may influence credit risk.

The goal is to perform exploratory data analysis (EDA), clean the data, engineer useful features and identify patterns that distinguish defaulted loans from successfully repaid loans.

---

## Dataset

The dataset used in this project contains historical loan information including borrower details, loan attributes and repayment outcomes.

Source:
https://www.kaggle.com/datasets/ranadeep/credit-risk-dataset

Key variables include:

* loan_amnt – loan amount requested
* funded_amnt – funded loan amount
* term – loan duration (36 or 60 months)
* int_rate – interest rate
* grade – loan grade assigned by the lender
* annual_inc – borrower annual income
* dti – debt-to-income ratio
* revol_util – revolving credit utilization
* open_acc – number of open credit lines
* total_acc – total number of credit accounts
* loan_status – loan outcome

---

## Project Workflow

### 1. Data Loading

The dataset is loaded using pandas and inspected to understand its structure, size and variable types.

### 2. Data Cleaning

Several columns required transformation before analysis:

* Converted **term** to numeric months
* Converted **interest rate** values to numeric format
* Cleaned **revolving utilization percentages**
* Transformed **employment length** into numeric years
* Created a **fico_mid** score from the FICO range

### 3. Target Variable Definition

A binary variable **default_flag** was created:

* 1 → Charged Off / Default
* 0 → Fully Paid

Other loan statuses were excluded to simplify the analysis.

### 4. Exploratory Data Analysis

Exploratory analysis was conducted to examine relationships between borrower characteristics and loan default.

The analysis includes:

* Loan amount distribution
* Default rate comparison
* Default distribution across loan grades
* Relationship between loan term and default
* Correlation analysis between numerical variables

### 5. Visualization

Several plots were created to better understand the patterns in the data:

* Default rate distribution
* Loan amount vs default
* Default rate by loan term
* Correlation heatmap of numeric variables

---

## Key Findings

Some general insights from the analysis include:

* Loans with longer terms tend to show higher default rates.
* Higher interest rates often correspond with increased credit risk.
* Borrowers with higher debt-to-income ratios appear more likely to default.
* Loan grade provides strong indication of repayment probability.

---

## Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook

---

## Files

credit_risk_analysis.ipynb – full exploratory data analysis and visualization notebook

---

## Author

Akhtar R. Khan
