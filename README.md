# Credit-Card_Fraud-Detection

This project is a simple program that compares Isolation Forest Algorithm and Local Outlier Factor (LOF) algorithm and finds out which one is better in detecting credit card fraud anomalies. 

The Dataset which I imported is from Kaggle and can be found at (https://www.kaggle.com/mlg-ulb/creditcardfraud)

The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, they cannot provide the original features and more background information about the data. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

My Final Observations from the experiment: 


Observations :
1. Isolation Forest detected 675 errors versus Local Outlier Factor detecting 935 errors.
2. Isolation Forest has a 99.74% accuracy and LOF has 99.67% accuracy. 
3. When comparing error precision & recall for the 2 models , the Isolation Forest performed much better than the LOF as we can see that the detection of fraud cases is around 35 % versus LOF detection rate of just 5 %.
4. So overall Isolation Forest Method performed much better in determining the fraud cases which is around 35%.
5. We can also improve on this accuracy by increasing the sample size or use deep learning algorithms however at the cost of computational expense.We can also use complex anomaly detection models to get better accuracy in determining more fraudulent cases.
