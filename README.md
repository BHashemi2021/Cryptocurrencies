
![header.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/header.png)

# Cryptocurrencies
Applying Unsupervised Machine Learning

## Background

#### 1- Cryptocurency
'Created first in 2009, Bitcoin has become a revolutionary digital currency as it enables peer-to-peer payments without a third party such as a bank. Built based on Blockchain technology, a digital public ledger (or a record-keeping system that maintains participants' identities in secure and (pseudo-)anonymous form information on each transaction) receives a unique "hash" (or identity) and is added to the end of the ledger (Figure 1). 

#### 2- A myriad of different cryptocurrencies
Blockchain technology is an open source technology, meaning any software developer can use the original source code and create something new. Developers have done just that. It is estimated to be more than 4,500 different cryptocurrencies to date, and the figure keeps increasing. In 2017, the number of cryptos surpassed 1,000' (1).  

#### Figure 1: How blockchain works

----------------------------

![blockchain.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/blockchain.png)

----------------------------
* Image courtesy of [PwC](https://www.pwc.com/us/en/industries/financial-services/fintech/bitcoin-blockchain-cryptocurrency.html)


## Purpose of the Analysis

We are creating an analysis for a clients who is preparing to get into the cryptocurrency market. This client is a senior manager for the Advisory Services Team at Accountability Accounting. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they have asked us to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The dataset, crypto_data.csv obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist), is not ideal for our purpose, so it will need to be processed to fit the machine learning models. Since there is no known output for what we are looking for, we would use unsupervised learning. To group the cryptocurrencies, we will employ cluster algorithm. Finally we would use data visualizations to share our findings with the board.

## What We are Creating
This task consists of four technical analysis, as they follow:

        1: Preprocessing the Data for PCA
        2: Reducing Data Dimensions Using PCA
        3: Clustering Cryptocurrencies Using K-means
        4: Visualizing Cryptocurrencies Results


### Preprocessing the Data for PCA

After keeping all the cryptocurrencies that are being traded, dropping the redundants columns, or the ones not used in clustering algorithms, removinge rows with at least one null value, etc, the dataframe looked like Figure 2.


#### Figure 2: The first cleaned DataFrame 

----------------------------

![1-crypto_DataFrame.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/1-crypto_DataFrame.png)

----------------------------

### Reducing Data Dimensions Using PCA

Applying the Principal Component Analysis (PCA) algorithm, we reduced the dimensions of the X DataFrame to three principal components and placed these dimensions in a new DataFrame (Figur 3).

#### Figure 3: Applying the Principal Component Analysis Algorithm

----------------------------

![2-pca_dataFrame.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/2-pca_dataFrame.png)

----------------------------


### 

Using the PCS DataFrame, we created an elbow curve using hvPlot to find the best value for K (Figure 4).


#### Figure 4: The elbow curve. 

----------------------------

![elbow_plot.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/elbow_plot.png)

----------------------------


### Clustering Cryptocurrencies Using K-means

Using the PCS DataFrame we ran the K-means algorithm to make predictions of the K clusters for the cryptocurrencies’ data and created a new DataFrame by concatenating the crypto_df and pcs_df DataFrames on the same columns (Figure 5).


#### Figure 5:  

----------------------------

![3-clustered_df.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/3-clustered_df.png)

----------------------------

### Visualizing Cryptocurrencies Results

 We finally, created a scatter plot with Plotly Express and hvplot to visualize the distinct groups that corresponded to the three principal components in 2-dimensional (Figure 6) and 3-dimensional plots (Figure 7).


#### Figure 6: The distinct groups that corresponded to the three principal components 


----------------------------

![hvplot.scatter_plot.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/hvplot.scatter_plot.png)


---------------------------



Figure 7: The Thre dimensional plot of the three components 

---------------------------

![3D_Scatter_with_Clusters.png](https://github.com/BHashemi2021/Cryptocurrencies/blob/main/Resources/Images/3D_Scatter_with_Clusters.png)

----------------------------


## Recommendations
The yellow outlier "BitTorrent" could be removed from dataset as its row contains only one item. 
The bulk of remaining cryptocurrencies and outliers may still need to be examined further by a financial expert for the kind of cryptocurrency and their function in the financial market (coin vs token). 


### Resources

        1- Google Colab
        2- Jupyter Notebook (Anaconda3)
        3- Microsoft CSV files 
        4- Python 3.9 (64-bit)
        5- VS Code Editor (64-1.58.2)
        

### References 

1- Types of Cryptocurrency, Nicholas Rossolillo, Aug 12, 2021 at https://www.fool.com/investing/stock-market/market-sectors/financials/cryptocurrency-stocks/types-of-cryptocurrencies/

