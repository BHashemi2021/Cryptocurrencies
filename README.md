# Cryptocurrencies
Unsupervised Machine Learning

## Background
<<<<<<< HEAD
We are creating an analysis for our clients who are preparing to get into the cryptocurrency market.

One of our most important clients is a senior manager for the Advisory Services Team at Accountability Accounting. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they have asked us to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data we will be working with with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what we are looking for, we would use unsupervised learning. To group the cryptocurrencies, we will employ cluster algorithm. Finally we would use data visualizations to share our findings with the board.

## What You're Creating
This new assignment consists of four technical analysis, as follows:

        1: Preprocessing the Data for PCA
        2: Reducing Data Dimensions Using PCA
        3: Clustering Cryptocurrencies Using K-means
        4: Visualizing Cryptocurrencies Results


### Preprocessing the Data for PCA



### Reducing Data Dimensions Using PCA



### Clustering Cryptocurrencies Using K-means


### Visualizing Cryptocurrencies Results





## Recommendations
The yellow outlier "BitTorrent" needs to be removed from dataset.
The outliers need to be excluded from the dataset as they are products other than cryptocurrencies, and they are built through blockchain processes.
=======

You and Martha have done your research. You understand what unsupervised learning is used for, how to process data, how to cluster, how to reduce your dimensions, and how to reduce the principal components using PCA. It’s time to put all these skills to use by creating an analysis for your clients who are preparing to get into the cryptocurrency market.

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.


### What You're Creating

    1: Preprocessing the Data for PCA
    2: Reducing Data Dimensions Using PCA
    3: Clustering Cryptocurrencies Using K-means
    4: Visualizing Cryptocurrencies Results

### 1: Preprocessing the Data for PCA

•	The following five preprocessing steps have been performed on the crypto_df DataFrame:
o	All cryptocurrencies that are not being traded are removed (3 pt)
o	The IsTrading column is dropped (3 pt)
o	All the rows that have at least one null value are removed (3 pt)
o	All the rows that do not have coins being mined are removed (3 pt)
o	The CoinName column is dropped (3 pt)
•	A new DataFrame is created that stores all cryptocurrency names from the CoinName column and retains the index from the crypto_df DataFrame (5 pt)
•	The get_dummies() method is used to create variables for the text features, which are then stored in a new DataFrame, X (5 pt)
•	The features from the X DataFrame have been standardized using the StandardScaler fit_transform() function (5 pt)




>>>>>>> 7a16abea82564c2a10281ccc65a2cfa6c7958628
