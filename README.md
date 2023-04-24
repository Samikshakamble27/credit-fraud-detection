# credit-fraud-detection
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Project Explanation:
1)Imported all the required libraries
2)loaded dataset into the csv format as pd to work on that dataset
3)get dataset information and check if there is missing values present in dataset or not
4)distribute the ligit transection and fraudulant transection data to work on training data
5)check the shape of both ligit and fraudulant transection
6) As we can see there is large amount of data present in ligit transection rather than fraudulant transection so we cannot feed this uneven data to our training data for that we need to balance data.
7) due to unbalanced data we can't use that as a training data
0 --> Normal transaction
1 --> Fraudulent Transaction
8)take random transactions from legit transection to make it balanced
9) now concatinate legit and fraud data. by conctinating both legit and fraud transection data new data will bw created 
10) splited new data into training data and testing data
11) for training model used logistic regression algorithm. regression algorithm used for binary classification problem.
12) Training the logistic regression model for Training Data
13) then check the accuracy of both training data and testing data
