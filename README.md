# KNN-Classification
K-Nearest Neighbors (KNN) is a supervised machine learning algorithm used for classification (and regression). It classifies a new data point based on the majority class among its k closest points in the training set.

How It Works
Choose a value of k (number of neighbors to consider).

For a new, unseen data point:

Calculate the distance from this point to all points in the training data.
(Commonly Euclidean distance, but Manhattan, Minkowski, etc. can also be used.)

Identify the k closest points (neighbors).

Assign the class label that is most frequent among these neighbors.

The prediction is purely based on training data — KNN stores the data instead of learning explicit parameters.

Key Points
Lazy Learning: No training phase — computation happens at prediction time.

Instance-Based: Keeps all training samples in memory.

Non-Parametric: Makes no assumptions about data distribution.

Why Normalization is Important
KNN relies on distances.

If features are on different scales (e.g., height in cm vs. weight in kg), large-scale features dominate the distance measure.

Solution: Apply Standardization or Min-Max scaling before using KNN.

Choosing k
Small k → More sensitive to noise (high variance).

Large k → Smoother decision boundary, but may misclassify minority classes.

Often chosen using cross-validation.

Advantages
Simple and easy to implement.

Works well for small datasets.

No assumptions about underlying data.

Disadvantages
Computationally expensive for large datasets.

Sensitive to irrelevant features and scaling.

Performance degrades with high-dimensional data (curse of dimensionality).


