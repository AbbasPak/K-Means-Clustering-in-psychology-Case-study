
******************
K-means clustering
******************


.. contents::
  :local:
  :depth: 3


**********
Motivation
**********
*K-means clustering* is a highly efficient and commonly used algorithm for partitioning data into clusters, providing a qualitative interpretation of the data by grouping similar conditions together. The algorithm calculates the similarity and dissimilarity among observations to determine cluster assignments. 
Fig1
The main objective of the K-means algorithm is to minimize the within-cluster sum of squares, also known as inertia or distortion. It quantifies the sum of squared distances between each data point and its assigned centroid within the cluster, known as within-cluster sum of squares (WCSS). The algorithm optimizes this objective function by iteratively updating the centroids and reassigning data points to clusters. 
The algorithm initially selects *k* data points randomly from the dataset as the initial centroids, which act as representatives of the clusters. For each data point, the algorithm calculates the distance between the point and each centroid. The data point is assigned to the cluster whose centroid is closest to it. The commonly used distance metric is Euclidean distance, although other metrics can be used. After assigning all data points to clusters, new centroids are computed for each cluster by taking the mean of the data points assigned to that cluster. This step updates the positions of the centroids. These steps are repeated until convergence is achieved. Convergence occurs when the centroids' positions stabilize (i.e., no significant change occurs between iterations) or when a maximum number of iterations is reached. Upon convergence, the algorithm outputs the final centroids and the assignment of each data point to a cluster, representing the resulting clusters obtained from the K-means algorithm.
An important aspect of this algorithm is the selection of the desired number of clusters, denoted as *k*. Several methods and heuristics exist to estimate the optimal number of clusters, such as the *elbow method* or *silhouette analysis*. The *elbow method* is a simple and intuitive technique that serves as a starting point for determining the optimal number of clusters in K-means clustering. This method relies on the observation that as the number of clusters increases, the WCSS typically decreases, as it measures the total distance between data points and their assigned cluster centroids. However, the decrease becomes less significant when the number of clusters becomes too large. To implement the elbow method, a range of values for *k* is chosen, starting with a small number and gradually increasing it. For each value of *k*, the K-means clustering algorithm is run, and the WCSS is calculated. A plot is then created with the number of clusters on the x-axis and the WCSS on the y-axis, often referred to as the elbow plot. The point on the plot where the WCSS starts to decrease at a slower rate is considered the elbow of the plot. The corresponding value of *k* at this point is considered the optimal number of clusters.





************
References
************

1. https://towardsdatascience.com/introduction-to-machine-learning-algorithms-linear-regression-14c4e325882a
2. https://machinelearningmastery.com/linear-regression-for-machine-learning/
3. https://ml-cheatsheet.readthedocs.io/en/latest/linear_regression.html
#. https://machinelearningmastery.com/implement-simple-linear-regression-scratch-python/
#. https://medium.com/analytics-vidhya/linear-regression-in-python-from-scratch-24db98184276
#. https://scikit-learn.org/stable/auto_examples/linear_model/plot_ols.html
#. https://scikit-learn.org/stable/modules/generated/sklearn.compose.TransformedTargetRegressor.html


