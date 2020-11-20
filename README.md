# Cryptocurrencies

A prominent investment bank is interested in offering investments in cyrptocurrencies.  The pourpose of this analysis is to determine what cryptocurrencies are on the market and to create a classification system for the new investment offering.  To accomplish this I have taken the following steps:

## Preprocessing
* Removing cryptocurrencies that are not being currently traded.
* Create variables for text features using get_dummies().
* Use StandardScaler to standardize the features.
* Drop columns that will not be used in the clustering algorithm.
* Apply PCA to extract three principal components.

## Clustering
* Use the principal components to create an elbow curve to determine the optimal number of clusters.
* Run K-means algorithm to make predictions for the clusters.
* Merge data frames to include all relevant information, including cluster/class for each cryptocurrency.

## Visualization
* Use Plotly Express to create a 3d scatter of the clusters.
* Create a sortable table containing all of the tradable cryptocurrencies.
* Create a new DataFrame that incluede the Total Coin Supply, Total Coins Mined, Name, and Class of each tradable cryptocurrency.
* Create a 2d scatter plot to visualise the tradable cryptocurrencies.
