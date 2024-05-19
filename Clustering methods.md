
# Clustering Methods

`Clustering` encompasses a wide range of techniques for identifying subgroups, or clusters, within a data set. 
The goal of clustering is to partition observations into distinct groups where the members of each group are highly similar to one another, yet significantly different from members of other groups. To achieve this, it’s essential to define what makes observations similar or different, which typically involves identifying patterns in an unlabeled data set, such as shape, size, color, or behavior. As an unsupervised learning method, clustering operates without predefined labels or guidance, analyzing the data independently.

<img src="figures/clusterfin.JPG" width="600" height="300"> 
[ref](https://www.javatpoint.com/clustering-in-machine-learning)



One practical application of clustering is in marketing, where we might analyze various metrics (e.g., median household income, occupation, proximity to urban areas) 
for a large population. The objective here is to perform market segmentation, grouping individuals into clusters that are more likely to respond 
to specific advertising strategies or purchase particular products. This segmentation process is effectively clustering the individuals in the data set.

Due to its widespread applicability, numerous clustering methods exist across different fields. Clustering methods are generally classified into 
Hard Clustering (where each data point belongs to only one group) and Soft Clustering (where data points can belong to multiple groups). 
However, several other approaches also exist. Key clustering methods in machine learning include:

1.	*Partitioning Clustering*: This method divides data into non-hierarchical groups, also known as centroid-based clustering. A common example is the `K-Means` algorithm, 
which partitions the data set into a predefined number of groups (k). 
Each cluster center is determined so that the distance between data points within a cluster is minimized compared to points in other clusters.

<img src="figures/clusterpar.JPG" width="600" height="300"> 
[ref](https://www.javatpoint.com/clustering-in-machine-learning)

3.	*Density-Based Clustering*: This approach connects dense regions of data into clusters, forming arbitrarily shaped distributions as long as dense regions are connected. 
By identifying high-density clusters separated by sparser areas, these methods can struggle with varying densities and high-dimensional data. 
An example is the `DBSCAN` algorithm.

<img src="figures/clusterden.JPG" width="600" height="300"> 
[ref](https://www.javatpoint.com/clustering-in-machine-learning)

4.	*Distribution Model-Based Clustering*: This method clusters data based on the probability of belonging to a particular distribution, 
often assuming Gaussian distributions. A notable example is the Expectation-Maximization algorithm using `Gaussian Mixture Models` (GMM).

5.	*Hierarchical Clustering*: Unlike partitioning methods, `hierarchical clustering` does not require a predefined number of clusters. 
Instead, it creates a tree-like structure (dendrogram) that illustrates the hierarchy of clusters. Clusters can be formed at any 
level by cutting the dendrogram at the appropriate point. The Agglomerative Hierarchical algorithm is a typical example.

6.	*Fuzzy Clustering*: In this soft clustering method, data objects can belong to multiple clusters, with membership coefficients indicating the degree of belonging. 
The Fuzzy C-Means algorithm, also known as `Fuzzy K-Means`, is an example.
These diverse clustering techniques enable the analysis and segmentation of data sets in various ways, each with its unique strengths and applications.

### Hierarchical Clustering

Hierarchical clustering develops the hierarchy of clusters in the form of a tree. This tree-shaped structure is known as *dendrogram*. In fact, dendrogram is a tree diagram that is used to show the arrangement of clusters produced by hierarchical clustering. Instead of receiving a "smooth" output of clusters, hierarchical clustering gives us a tree of clusters. When trying to learn a hierarchy from data, there are two approaches:

+ Agglomerative: It is a bottom-up approach in which the algorithm is performed by taking all data points as individual clusters and merging them until one cluster remains.
+ Divisive: This approach is the opposite of the agglomerative approach and is top-down. That is, it starts with all items in a cluster and recursively divides them into clusters until each item is in its own cluster.

### References

1. https://www.javatpoint.com/k-means-clustering-algorithm-in-machine-learning
2. Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani, (2013). 
An introduction to statistical learning : with applications in R. New York :Springer.







