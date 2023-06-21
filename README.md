## CryptoClustering

Use your knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes

### Find the Best Value for k Using the Original Scaled DataFrame
- Use the elbow method on the PCA data
 - Create a list with the number of k values from 1 to 11.
 - Create an empty list to store the inertia values.
 - Create a for loop to compute the inertia with each possible value of k.
 - Create a dictionary with the data to plot the elbow curve.
 - Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

### Cluster Cryptocurrencies with K-means Using the Original Scaled Data
- Cluster the cryptocurrencies for the best value for k on the original scaled data
 - Initialize the K-means model with the best value for k.
 - Fit the K-means model using the PCA data.
 - Predict the clusters to group the cryptocurrencies using the PCA data.
 - Create a copy of the original data and add a new column with the predicted clusters.
 - Create a scatter plot using hvPlot

### Optimize Clusters with Principal Component Analysis
 - Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components
 - Retrieve the explained variance to determine how much information can be attributed to each principal component
 - Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

#### Answer the following questions:
- What is the best value for k?
- What is the total explained variance of the three principal components?
- What is the best value for k when using the PCA data?
- Does it differ from the best k value found using the original data?
- What is the impact of using fewer features to cluster the data using K-Means?
