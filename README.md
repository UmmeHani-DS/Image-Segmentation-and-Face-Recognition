# Image Segmentation and Face Recognition

### Introduction
This project encompasses two main tasks: interactive foreground segmentation using K-Means clustering, and face recognition using k-Nearest Neighbors (k-NN). These tasks involve the application of machine learning techniques for image processing and pattern recognition.

## Q1: Interactive Foreground Segmentation Using K-Means Clustering
The goal is to implement a basic version of the interactive image cut-out/segmentation approach called Lazy Snapping. This involves:
1. **K-Means Clustering**: Write a function to perform K-Means clustering on color pixels.
2. **Seed Pixel Extraction**: Extract foreground and background seed pixels from human annotations.
3. **Cluster Likelihood Calculation**: Compute the likelihood of a pixel belonging to a cluster.
4. **Class Assignment**: Assign each pixel to the foreground or background class based on the calculated likelihoods.
5. **Result Analysis**: Compare results for different cluster numbers (N) and report the findings.

### Implementation Steps
1. **K-Means Clustering Function**: Implement a function that takes the desired number of clusters (k) and data points, outputting cluster indices and centroids.
2. **Seed Pixel Extraction**: Extract foreground and background pixels from provided auxiliary images.
3. **Likelihood Computation**: Calculate the likelihood of each pixel belonging to each cluster using an exponential function.
4. **Pixel Classification**: Assign pixels to foreground or background based on the computed likelihoods.
5. **Result Comparison**: Evaluate results for different values of N (e.g., N=64) and document the findings.

## Q2: Face Recognition Using K-NN
The second task involves using a simplified version of the CMU Pose, Illumination, and Expression (PIE) dataset to implement face recognition. The dataset contains 10 subjects with 170 images each, resized to 32x32 pixels.

### Implementation Steps
1. **Data Pre-processing**: Normalize each face image vector to unit length. Split the data into training (150 images per subject) and testing (20 images per subject) sets.
2. **K-NN Classifier Implementation**: Implement a k-NN classifier from scratch, using both Euclidean and cosine similarity distance measures for different values of k.
3. **Performance Evaluation**: Evaluate the k-NN classifier with varying training set sizes and different k-values (2, 5, 7, and 11).
4. **Comparative Analysis**: Use Sklearn to apply SVM and GaussianNB classifiers on the dataset and compare their accuracy with the k-NN classifier.
5. **Dimensionality Reduction**: Perform PCA on the dataset and visualize the training and testing sets in 3-D space using matplotlib or Seaborn.

### Tasks
1. **Data Normalization and Splitting**: Normalize face image vectors and split the dataset into training and testing sets.
2. **k-NN Classifier**: Implement k-NN classifier with Euclidean and cosine similarity measures.
3. **Performance Evaluation**: Test the classifier with different k-values and report the results.
4. **Comparison with SVM and GaussianNB**: Apply SVM and GaussianNB classifiers and compare their accuracy with k-NN.
5. **PCA Visualization**: Perform PCA and visualize the datasets in 3-D space.
