## Elbow method for K-means:
1. Initially one has to start at K=2, assuming there are only two clusters. And calculate the respective cost.
2. Increase the K value by 1, and calculate the cost again.
3. Repeat the above step till we find the "Elbow point", or the value of K at which there is a drastic drop in the cost value.
4. After this point the cost converges to a value. This is the required number of clusters.

## DBSCAN clusters using Silhouette method
1. Generally the number of min points would be greater than or equal to the dimensionality of the dataset.
2. For every entry in the dataset, find the average distance between all other points in the cluster.
3. Measure the distance between each point and points in other clusters.
4. Calculate the score by differencing both the averages and dividing with the largest. 
5. The number of clusters for which the score is the highest and closest to 1 should be chosen.