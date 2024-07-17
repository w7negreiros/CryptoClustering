# Clustering Cryptocurrencies - UofT Data Analytics - Bootcamp

In this project I apply the unsupervised learning technique of K-Means clustering to group cryptocurrencies by their performance in an effort to create profitable portfolio recommendations.

# Data Used

[crypto_market_data.csv](Resources/crypto_market_data.csv) - market data of different cryptocurrencies during different time periods

# Summary

I start by using the elbow curve method, using normalized data, to find the optimal k value for the K-Means model that will use all of the original features of the dataset.

image 1

Then, using the optimal k value I train and predict the K-Means model to generate 4 clusters of cryptocurrencies. The inertia of each cluster was significant enough to consider reducing the amount of features.

image 2

To reduce the amount of features used, I applied Principal Component Analysis to create 3 primary clusters.

image 3

I then used the PCA data to again calculate the optimal k value for the K-Means model.

image 4

Finally, with the optimal k value for the PCA features, I plot the new clusters.

image 5

# Technologies

This is a Python 3.7 project ran using a JupyterLab in a conda dev environment.

The following dependencies are used:

Jupyter - Running code 
Conda (4.13.0) - Dev environment    
Pandas (1.3.5) - Data analysis  
Matplotlib (3.5.1) - Data visualization 
Numpy (1.21.5) - Data calculations + Pandas support     
hvPlot (0.8.1) - Interactive Pandas plots   
scikit-learn (1.0.2) - KMeans clustering, data normalization, and PCA   

# Usage
The Jupyter notebook [crypto_investments.ipynb](Crypto_Clustering.ipynb) will provide all steps of the data collection, preparation, and analysis. Data visualizations are shown inline and accompanying analysis responses are provided.

