# Stock Analysis Using Data Clustering
### Group project for CIS 600 - Fundamentals of Data & Knowledge Mining
  
  
*Group Members: Ashraf Elnashar, Gregory Shin, Gafei Szeto*

**Goal:** To use clustering techniques with historical stock prices to group different stocks together, in order to form an investment strategy.

**Dataset:**

*source: <https://www.kaggle.com/tsaustin/us-historical-stock-prices-with-earnings-data#dataset_summary.csv>*

*Description:*
 
1. dataset_summary.csv: Summary table for all stocks in this dataset.
2. earnings_latest.csv: Earnings data for each stock with earnings date, estimated EPS and reported EPS.
3. stock_prices.csv: Daily stock price data with open, close, low, high, trading volumes and adjusted closing prices as well as stock split coefficient.
4. dividends_latest.csv: Dividend data for each stock with dividend date.

##Introduction

The ultimate goal in creating a stock portfolio is to gather a group of stocks that will increase in value over time. However, it is often difficult to pick which stocks to invest in from all the ones that are available. Therefore, we intend to explore the use of clustering analysis in identifying groups of similarly performing stocks.

##Goal
To use historical stock prices to determine patterns that will allow us to group together various stocks by performance. Possible groupings may be stocks that perform above average or below average, and stocks that rise in value together, or drop in value together.

## Details
**Clustering Types Expected**

Various clustering techniques will need to be used in order to find the ideal model for stock group discovery. Some potential techniques are:

* Partitional clustering - Stocks will be sorted into discrete groups with no overlap and no subgroups. Two potential groups are over-performing stocks and under-performing stocks.
* Hierarchical clustering - It may be possible that stocks will be found, during discovery, to have subgroups. Clusters may be defined as over-performing and under-performing stocks, with subgroups being defined by various levels of performance.

**Potential Clustering Techniques:**

* K-Means - By using a prototype-based clustering technique, a centroid can be defined which may be used to sort stocks into over-performing and under-performing groups.
* Divisive Approach - By starting with one cluster, and by identifying arbitrary dividing lines, the cluster can be divided into multiple clusters that can satisfy the desired conditions.