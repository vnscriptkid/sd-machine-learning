# Kmeans clusterning
- Unsupervised learning
- Find patterns in data -> Draw insights
- Categorize data points into K clusters
    - There's different ways to group data points into K clusters
    - Goal is to minimize the distance between data points in the same cluster and maximize the distance between data points in different clusters
- Iterative process
    - Randomly assign data points to K clusters
    - Calculate the centroid of each cluster
    - Calculate the distance between each data point and the centroid of its cluster
    - Assign each data point to the cluster with the closest centroid
    - Repeat steps 2-4 until the clusters do not change

## Misc
- Literally, everything is a data point. e.g. a person, a house, a transaction...
- Data point:
    - 1 dimension: line
    - 2 dimension: 2d (x, y)
    - 3 dimension: 3d (x, y, z)
    - n dimension: vector(x1, x2, x3, ..., xn) -> where n is the number of features (age, gender, income, etc.)
- How to calculate distance between data points?
    - Euclidean distance:
        - 1 dimension: |x1 - x2|
        - 2 dimension: sqrt((x1 - x2)^2 + (y1 - y2)^2)
        - 3 dimension: sqrt((x1 - x2)^2 + (y1 - y2)^2 + (z1 - z2)^2)
        - n dimension: sqrt((x1 - x2)^2 + (x2 - x3)^2 + ... + (xn - x1)^2)
- How to choose new centroids from the existing clusters? Calculate geometric mean of the data points in the cluster
- How to determine the optimal number of clusters?

## Ref
- https://youtu.be/lX-3nGHDhQg?si=okTjWn4hCtGCApGl