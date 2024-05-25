---
title: "Unsupervised Learning Models I experienced with"
tags:
    - AI
    - Scikit-learn
    - Developer
date: "2024-03-10"
thumbnail: "/assets/img/thumbnail/kMeans.png"
bookmark: true
---

# Unsupervised Learning: Exploring Key Techniques
---

## Principal Component Analysis (PCA)
---
PCA is a dimensionality reduction technique that identifies the most important features in your data. It's commonly used for feature extraction, noise reduction, and visualization.

### How to Use PCA:
1. Standardize your data.
2. Compute the covariance matrix.
3. Calculate the eigenvectors and eigenvalues.
4. Select the top-k eigenvectors as your principal components.
5. Transform your data using these components.

## K-Means Clustering
---
K-Means groups similar data points into clusters. It's useful for customer segmentation, anomaly detection, and recommendation systems.

### How to Use K-Means:
1. Choose the number of clusters (k).
2. Initialize k centroids randomly.
3. Assign each data point to the nearest centroid.
4. Update centroids based on the mean of assigned points.
5. Repeat steps 3 and 4 until convergence.

## Gaussian Mixture Models (GMM)
---
GMM represents data as a mixture of Gaussian distributions. It's great for density estimation, anomaly detection, and image segmentation.

### How to Use GMM:
1. Initialize the model with random parameters.
2. Expectation-Maximization (EM) algorithm:
   - E-step: Compute the probability of each data point belonging to each Gaussian component.
   - M-step: Update the model parameters (means, covariances, and weights).
3. Repeat the EM steps until convergence.

## Hierarchical Clustering
---
Hierarchical Clustering builds a tree-like structure of data points. It's useful for visualizing relationships and creating dendrograms.

### How to Use Hierarchical Clustering:
1. Start with each data point as a separate cluster.
2. Merge clusters based on similarity (e.g., single linkage, complete linkage).
3. Continue merging until all points belong to a single cluster or meet a stopping criterion.

## Autoencoders
---
Autoencoders are neural networks used for unsupervised feature learning and data compression.

### How to Use Autoencoders:
1. Encode input data into a lower-dimensional representation (latent space).
2. Decode the latent representation back to the original data.
3. Train the autoencoder to minimize the reconstruction error.
