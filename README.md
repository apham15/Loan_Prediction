## **Loan_Prediction**

Lending Club is "the world's largest online marketplace connecting borrowers and investors." It is a peer-to-peer lending network that open sources some of its loan data to the community.

I use the loan.csv file that contains real-world, historical data on loans organized by Lending Club between 2007 and 2011.

![Screen Shot 2020-10-13 at 11 01 14 PM](https://user-images.githubusercontent.com/63126292/95942130-01280980-0da8-11eb-88a8-cfa750120469.png)

1. Business Understanding

You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The dataset given contains the information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

![Screen Shot 2020-10-13 at 11 33 17 PM](https://user-images.githubusercontent.com/63126292/95943851-89101280-0dac-11eb-85c6-39e7db5ef5b4.png)

2. Business Concept
When a person applies for a loan, there are two types of decisions that could be taken by the company:

Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

a. Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

b. Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

c. Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

3. In this project, I did perform all the basic but necessary steps that make the audience to understand EDA process. Then, I apply Supervised Learning Models to predict the loan status with all the features.

a. Understand the data:

* Import libraries and dataset
* Understand the data
* Apply descriptive analysis and visualization to give some insigh of the raw data

b. EDA:

* The target (Loan Status) is divided by Good Loan and Bad Loan
* Determine the features by grouping categorical and numerical features
* Eliminate the unuseful categorical features
* Adjust data format
* Clean the data 
* Apply SimpleImputer, MaxAbsScaler, and LabelEncoder to fill in NaN values
* Transform data by using RobustScaler, StandardScaler, and OneHotEncoder
* Apply feature engineering (PCA)
* Utilize hstackto make the final train and test dataset to combine PCA, Discreate columns, and Spare columns

4. Machine Learning Algorithms
* Utilize Logistic Regression, K-Nearest Neighbor Classifier, Decision Tree Classifier, Random Forest Classifier, Naive Bayes Classifier, Support Vector Classifier, Gradient Boosting Classifier to determine the preditction
* The best performance models are Gradient Boosting Classifier (87.57% accuracy) and Random Forest Classifier (87.29% accuracy)
* Apply GridSearchCV for tunning and find out the best GBM parameter is {'max_depth': 15, 'max_features': 'auto', 'n_estimators': 15} and the best Random Forest parameter is {'max_depth': 38, 'max_features': 'sqrt', 'n_estimators': 50}
* The optimized model achieved an ROCs are 99.5% (GBM) and 100% (Random Forest)
![download (21)](https://user-images.githubusercontent.com/63126292/97232670-93b6a880-17ab-11eb-8888-c68c20ca49f9.png)
![download (22)](https://user-images.githubusercontent.com/63126292/97232723-b21ca400-17ab-11eb-88d3-a48bdcc8db28.png)

5. Link of the dataset 
https://media.githubusercontent.com/media/apham15/large_csv/main/loan.csv'

6. My work
https://github.com/apham15/Loan_Prediction/blob/main/Supervised_Learning_Project_Loan_Prediction_final_version.ipynb
