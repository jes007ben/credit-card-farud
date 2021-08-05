# credit-card-fraud

Problem Statement:

The Credit Card Fraud Detection Problem includes modeling past credit card transactions with the knowledge of the ones that turned out to be fraud. This model is then used to identify whether a new transaction is fraudulent or not. Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications.
DataSet :

The dataset that is used for credit card fraud detection is derived from the following Kaggle URL : https://www.kaggle.com/mlg-ulb/creditcardfraud
Exploratory Data Analysis:

The data set is highly skewed, consisting of 492 frauds in a total of 284,807 observations. This resulted in only 0.172% fraud cases. This skewed set is justified by the low number of fraudulent transactions. The dataset consists of numerical values from the 28 ‘Principal Component Analysis (PCA)’ transformed features, namely V1 to V28. Furthermore, there is no metadata about the original features provided, so pre-analysis or feature study could not be done. The ‘Time’ and ‘Amount’ features are not transformed data. There is no missing value in the dataset. Model used : Isolation Forest, Support Vector Machine, Local Oulier Factor.
Conclusion:

    Isolation Forest detected 73 errors versus Local Outlier Factor detecting 97 errors vs. SVM detecting 8516 errors
    Isolation Forest has a 99.74% more accurate than LOF of 99.65% and SVM of 70.09
    When comparing error precision & recall for 3 models , the Isolation Forest performed much better than the LOF as we can see that the detection of fraud cases is around 27 % versus LOF detection rate of just 2 % and SVM of 0%.
    So overall Isolation Forest Method performed much better in determining the fraud cases which is around 30%.
    We can also improve on this accuracy by increasing the sample size or use deep learning algorithms however at the cost of computational expense.We can also use complex anomaly detection models to get better accuracy in determining more fraudulent cases
