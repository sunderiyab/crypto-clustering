# crypto-clustering
 # Cryptocurrency Clustering Analysis

This repo contains code and data for performing a clustering analysis on cryptocurrency market data using K-Means clustering and Principal Component Analysis (PCA). The goal of the analysis is to identify patterns and group cryptocurrencies based on their price changes using unsupervised learning

 # Dataset
 
The dataset used for this analysis is sourced from the crypto_market_data.csv file, which contains historical market data for various cryptocurrencies. The dataset includes columns such as price_change_percentage_24h, price_change_percentage_7d, price_change_percentage_14d, price_change_percentage_30d, price_change_percentage_60d, price_change_percentage_200d, and price_change_percentage_1y. These columns represent the percentage changes in cryptocurrency prices over different time periods.
<img width="715" alt="Screenshot 2023-06-19 at 2 03 03 PM" src="https://github.com/sunderiyab/crypto-clustering/assets/123790798/b0f1e2d0-f073-49c7-94b9-429bc50ff899">


# Codes/ Librarier

The code uses the following libraries:

Pandas: for data manipulation and analysis.
Scikit-learn: for implementing K-Means clustering and PCA.
HvPlot: for data visualization.

Data Preprocessing
K-means Clustering
Principal Component Analysis
Visualization



# Results
The optimal number of clusters is determined to be 2 or 3 based on the Elbow Method.
<img width="648" alt="Screenshot 2023-06-19 at 2 03 12 PM" src="https://github.com/sunderiyab/crypto-clustering/assets/123790798/6551d526-1c28-46e2-b0a4-35847c7be6b5">


Principal Component Analysis (PCA) is used to reduce the dimensionality of the data. The first three principal components capture approximately 89% of the total variance in the dataset
explained_variance_ratio = pca.explained_variance_ratio_
total_explained_variance = np.sum(explained_variance_ratio[:3])
print(f"The total explained variance of the three principal components is: {total_explained_variance}")

Scatter plots and composite plots are created to visualize the clusters and contrast the clustering results based on different techniques
<img width="648" alt="Screenshot 2023-06-19 at 2 03 21 PM" src="https://github.com/sunderiyab/crypto-clustering/assets/123790798/c8ab0a8e-9f33-42d1-b251-a159617c445b">


