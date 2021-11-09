# Cryptocurrency Clusters

## Background

* Created a report that includes what cryptocurrencies are on the trading market and determine whether they can be grouped to create a classification system for this new investment.

* Process data to fit the machine learning models. Since there is no known classification system, you will need to use unsupervised learning. You will use several clustering algorithms to explore whether the cryptocurrencies can be grouped together with other similar cryptocurrencies. You will use data visualization to share your findings with the investment bank.

## Instructions

### Data Preparation

* Read `crypto_data.csv` into Pandas. The dataset was obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist).

* Discarded all cryptocurrencies that are not being traded. In other words, filter for currencies that are currently being traded. Once you have done this, drop the `IsTrading` column from the dataframe.

* Removed all rows that have at least one null value.

* Filtered for cryptocurrencies that have been mined. That is, the total coins mined should be greater than zero.

* Converted features with text values into numerical data.

* Standardized dataset so that columns that contain larger values do not unduly influence the outcome.

### Dimensionality Reduction

* Performed dimensionality reduction with PCA. Preserved 90% of the explained variance in dimensionality reduction. How did the number of the features change?

* Reduced the dataset dimensions with t-SNE.

### Cluster Analysis with k-Means

* Created an elbow plot to identify the best number of clusters. 

### Recommendation

* Based on my findings, there is not a clear pattern of cryptocurrency clusters. Cryptocurrencies cannot be clustered together. 

