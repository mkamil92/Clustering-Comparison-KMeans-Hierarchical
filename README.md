# Clustering Comparison: K-Means vs. Hierarchical Clustering

## Overview

This repository contains a comparison of two clustering algorithms—K-Means and Hierarchical Clustering—applied to a shopping mall customer dataset. The aim of this project is to evaluate and compare the performance of these clustering methods in segmenting customers based on their attributes, including annual income, age, and spending score.

## Dataset

The dataset used for this project is from a shopping mall, containing information about customer demographics and behavior. The main features include:

- **Annual Income**: The annual income of the customer.
- **Age**: The age of the customer.
- **Spending Score**: A spending score assigned to the customer, reflecting their purchasing behavior.

## Clustering Algorithms

### K-Means Clustering

- K-Means clustering is a centroid-based algorithm where each data point is assigned to the nearest cluster center, and the cluster centers are iteratively adjusted until convergence.
- In this project, K-Means is applied to identify distinct customer segments based on annual income, age, and spending score.

### Hierarchical Clustering

- Hierarchical clustering builds a tree of clusters (dendrogram) by either successively merging clusters (agglomerative) or splitting them (divisive).
- Agglomerative hierarchical clustering is used in this project to identify clusters by iteratively merging the closest data points.

## Results

### Silhouette Score Comparison:

- **Silhouette Score - Hierarchical Clustering**: 0.21
- **Silhouette Score - K-Means Clustering**: 0.29

The silhouette score indicates how well-separated the clusters are. A higher silhouette score suggests better-defined clusters. In this case, K-Means performed slightly better than Hierarchical Clustering.

### Differences:

- **Hierarchical Clustering**: This method may capture different patterns in the data due to its merging approach, where clusters are created by progressively merging data points. It might reveal more subtle patterns that K-Means does not capture.
- **K-Means Clustering**: K-Means directly assigns points to clusters based on proximity to the centroids, which results in more well-defined, but sometimes less nuanced, customer segments.

### K-Means Cluster Centers Radar Chart:

- A radar chart shows the average values of the three features (Annual Income, Age, and Spending Score) for each of the six clusters identified by K-Means.
- The chart reveals significant overlap between the clusters, indicating that they are not well-separated and may not represent distinct customer segments.
