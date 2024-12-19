# Unsupervised-machine-learning


# Cryptocurrency Clustering with K-Means and PCA

Cluster cryptocurrencies using K-Means and Principal Component Analysis (PCA). This project involves normalizing the data, identifying optimal clustering parameters, and visualizing the results.

Prerequisites

Install the following libraries:

pandas

numpy

scikit-learn

hvplot

Steps

1. Normalize the Data

Input: Cryptocurrency data from a CSV file.

Process: Normalize the data using StandardScaler().

Output: Scaled DataFrame with "coin_id" as the index.

2. Find the Best k (Original Scaled Data)

Use the elbow method:

Create k values from 1 to 11.

Compute inertia for each k.

Plot an elbow curve to find the optimal k.

3. Cluster Cryptocurrencies (Original Data)

Steps:

Initialize and fit a K-Means model with the best k.

Add cluster labels to the scaled DataFrame.

Create a scatter plot using hvPlot:

x: price_change_percentage_24h

y: price_change_percentage_7d

Color points by clusters.

4. Use PCA for Optimization

Reduce features to 3 principal components using PCA.

Output: PCA DataFrame with "coin_id" as the index.

Question: What is the total explained variance of these components?

5. Find the Best k (PCA Data)

Repeat the elbow method on the PCA DataFrame.

Compare the best k with the value from the original scaled data.

6. Cluster Cryptocurrencies (PCA Data)

Steps:

Fit a K-Means model using the PCA DataFrame.

Add cluster labels to the PCA DataFrame.

Create a scatter plot using hvPlot:

x: PC1

y: PC2

Color points by clusters.

Key Questions

What is the best k for the original data and PCA data?

How does PCA impact clustering results?

Deliverables

Normalized DataFrame.

Elbow curves for original and PCA data.

Scatter plots of clusters.

Analysis of results.


