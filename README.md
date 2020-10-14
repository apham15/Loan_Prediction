## **Loan_Prediction**

Lending Club is "the world's largest online marketplace connecting borrowers and investors." It is a peer-to-peer lending network that open sources some of its loan data to the community.

I use the loan.csv file that contains real-world, historical data on loans organized by Lending Club between 2007 and 2011.

![Screen Shot 2020-10-13 at 11 01 14 PM](https://user-images.githubusercontent.com/63126292/95942130-01280980-0da8-11eb-88a8-cfa750120469.png)

1. Business Understanding

You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The dataset given contains the information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

1. In this project, I did perform all the basic but necessary steps that make the audience to understand EDA process. Then, I apply Supervised Learning Models to predict the loan status with all the features.

* Import libraries and dataset
* Understand the data
* Apply descriptive analysis and visualization to give some insigh of the raw data
* Determine the features and the target (Loan Status)
* Clean the data 
* Apply feature engineering (PCA)
* Use Logistic Regression, Decision Tree, and Random Forest Models to determine the preditction
* Conclude the best model that fit the dataset is Randome Forest with 96% accuracy

2. Link of the dataset 
https://media.githubusercontent.com/media/apham15/large_csv/main/loan.csv'

3. My work
https://github.com/apham15/Loan_Prediction/blob/main/Supervised%20Learning%20Project%20%20-%20final%20version.ipynb
