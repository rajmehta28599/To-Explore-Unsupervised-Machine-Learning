# To-Explore-Unsupervised-Machine-Learning

To explore #Unsupervised #machinelearningFrom the given ‘Iris’ dataset, predict the optimum number of clusters and represent it visually.

Unsupervised learning is a branch of machine learning that learns from test data that has not been labeled, classified or categorized. Instead of responding to feedback, unsupervised learning identifies commonalities in the data and reacts based on the presence or absence of such commonalities in each new piece of data. Alternatives include supervised learning and reinforcement learning.

For us, we are going to take a very basic example, and try to understand how this works! We are going to be working with a built-in dataset from sklearn: The Iris Dataset!
Sepal length in cm
Sepal width in cm
Petal length in cm
Petal width in cm
class:
Iris Setosa
Iris Versicolour
Iris Virginica

Algorithm:
We are going to be using a clustering algorithm:
Clustering is a method of unsupervised learning and is a common technique for statistical data analysis used in many fields. In Data Science, we can use clustering analysis to gain some valuable insights from our data by seeing what groups the data points fall into when we apply a clustering algorithm.
In particular we are going to use K-Means
Kmeans is one of the most popular “clustering” algorithms. K-means stores k centroids that it uses to define clusters. A point is considered to be in a particular cluster if it is closer to that cluster’s centroid than any other centroid.
K-Means finds the best centroids by alternating between (1) assigning data points to clusters based on the current centroids (2) choosing centroids (points which are the center of a cluster) based on the current assignment of data points to clusters.

Full Algorithm Definition
The Κ-means clustering algorithm uses iterative refinement to produce a final result. The algorithm inputs are the number of clusters Κ and the data set. The data set is a collection of features for each data point. The algorithms starts with initial estimates for the Κ centroids, which can either be randomly generated or randomly selected from the data set. The algorithm then iterates between two steps:
1. Data assignment step:
Each centroid defines one of the clusters. In this step, each data point is assigned to its nearest centroid, based on the squared Euclidean distance. More formally, if ci is the collection of centroids in set C, then each data point x is assigned to a cluster based on
Image for post
where dist( · ) is the standard (L2) Euclidean distance. Let the set of data point assignments for each ith cluster centroid be Si.
2. Centroid update step:
In this step, the centroids are recomputed. This is done by taking the mean of all data points assigned to that centroid’s cluster.
Image for post
The algorithm iterates between steps one and two until a stopping criteria is met (i.e., no data points change clusters, the sum of the distances is minimized, or some maximum number of iterations is reached).
This algorithm is guaranteed to converge to a result. The result may be a local optimum (i.e. not necessarily the best possible outcome), meaning that assessing more than one run of the algorithm with randomized starting centroids may give a better outcome.

https://towardsdatascience.com/unsupervised-machine-learning-9329c97d6d9f
