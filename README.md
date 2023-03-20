# CryptoClustering

I used unsupervised learning in Python to analyze whether changes in cryptocurrency prices over 24 hours or 7 days were related. Here's a summary of the steps I followed:

- Normalized the data from a CSV file using the StandardScaler() module from scikit-learn.

- Determined the optimal value for k using the elbow method on the original scaled DataFrame.

- Applied K-means clustering with the best value for k to the original scaled data, thereby clustering the cryptocurrencies.

- Optimized the clustering further by performing Principal Component Analysis (PCA) and reducing the features to three principal components.

- Repeated the same steps as the K-means model, but this time using the reduced features.

Based on my analysis, I concluded that using fewer features would yield similar results to the original model, as the same number of clusters were identified. However, in terms of inertia, the PCA model performed better.


![elbow_curve](https://user-images.githubusercontent.com/115505106/226489034-763a1176-7b44-4ef4-a1db-d3f092614799.png)
![elbow_curve_pca](https://user-images.githubusercontent.com/115505106/226489074-eed9b4af-c916-45ca-9bab-58b6652af8dd.png)

![kmeans_original](https://user-images.githubusercontent.com/115505106/226489048-6d497a72-ef14-4acf-b558-ff56e274cbdb.png)
![kmeans_pca](https://user-images.githubusercontent.com/115505106/226489083-c422a22f-4f43-44a5-92df-7124187ed08e.png)
