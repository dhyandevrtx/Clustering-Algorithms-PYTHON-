# Clustering-Algorithms-PYTHON-
Clustering Algorithms on the Iris Dataset
This project applies two clustering algorithms (KMeans and Hierarchical Clustering) to the Iris dataset, a classic dataset used in machine learning and clustering tasks. The goal is to explore unsupervised learning techniques to find natural groupings in the data.

Dataset
The Iris dataset contains measurements of four features (sepal length, sepal width, petal length, and petal width) for three species of Iris flowers (Setosa, Versicolour, and Virginica). However, for clustering, we do not use the species labels. The features are used to group the data points into clusters.

Key Components
Loading and Preprocessing:

The Iris dataset is loaded using sklearn.datasets.load_iris.
The species labels are ignored, as this is an unsupervised learning problem.
Clustering Algorithm Implementation:

KMeans Clustering: A centroid-based clustering algorithm that partitions the data into k clusters by minimizing the sum of squared distances to the centroids. The algorithm is applied with k=3, assuming 3 clusters corresponding to the 3 species in the dataset.
Hierarchical Clustering: An agglomerative method that builds a tree-like structure (dendrogram) to represent the nested groupings of the data. We also apply this algorithm with n_clusters=3.
Visualization:

The clusters are visualized using the first two features (sepal length and sepal width) for 2D visualization.
For KMeans, the centroids are marked on the plot to show the cluster centers.
For Hierarchical Clustering, the data points are grouped into three clusters.
Algorithms
KMeans Clustering
Description: KMeans clustering assigns data points to the nearest cluster centroid and updates the centroids iteratively. It is a simple and widely used algorithm for clustering tasks.
Why Suitable for Iris Dataset: KMeans is suitable because the Iris dataset consists of numerical features, and we want to identify the natural groupings within the data. With 3 distinct species, KMeans can effectively divide the data into 3 clusters.
Hierarchical Clustering
Description: Hierarchical clustering creates a tree of clusters by either iteratively merging smaller clusters (agglomerative) or splitting larger clusters (divisive). It does not require specifying the number of clusters in advance.
Why Suitable for Iris Dataset: Hierarchical clustering is effective for smaller datasets like Iris, as it helps visualize the relationship between data points and how they are grouped at different levels of granularity.

Conclusion
This project demonstrates the application of unsupervised learning techniques (KMeans and Hierarchical Clustering) to the Iris dataset. Both clustering algorithms are effective for identifying natural groupings in the dataset, even though the true species labels were not used during the clustering process.

License
This project is licensed under the MIT License - see the LICENSE file for details.
