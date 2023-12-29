# Cleaning and Preprocessing Loan Data using NumPy

## Data and Tools Used

**Data**
- loan-data.csv (containing 10000 rows of data with the fields - id, issue_d, loan_amnt, loan_status, funded_amnt, term, int_rate, installment, grade, sub_grade, verification_status, url, 
                 addr_state and total_pymnt)
- Loan Dataset Dictionary.xlsx (file describing the data contained in each of the fields)
- EUR-USD.csv (file containing the monthly average conversion rates between the 2 currencies - to be used for creating additional columns with data in Euros)

**Data Cleaning & Preprocessing** - Python, NumPy (using Jupyter Notebook)

## Task:

Clean the loan data and preprocess it to be in a form which can then be used to calculate the probabilities of default associated with every account/client in a Credit Risk Model

## Summary:

The complete details of each step taken are captured in the attached Jupyter Notebook with appropriate comments. Below is a brief summary/overview:

Imported the raw data in an nd-array and performed the following:
- Split the dataset into 2 subparts (numeric and non-numeric)
- Checked for and filled out missing values
- Manipulated columns containing text data to strip any redundant text and converted them to numeric data wherever possible by grouping the categories
- Manipulated columns containing numeric data and added new ones displaying the default amounts(USD) in EUR
- Saved the data into .npz files at various checkpoints to ensure it was not lost
- Finally, merged the datasets and the headers into a final comprehensive text file
