# Semi-superwised-learning-for-image-classification
This repository contains an implementation of semi-supervised learning using K-Means clustering on the Fashion MNIST.

## Steps
In this project, we:
-  Apply K-Means clustering to the Fashion MNIST and Overhead MNIST datasets.
-  Experiment with different values of K (40 and 50).
-  Select a subset of images within a specified frequency threshold to label according to the cluster center.
-  Train a neural network (multi-layer perceptron, MLP) model using the labeled subset.
-  Evaluate the model on unseen data that was not involved in the clustering process and further classification process.

## Result
Best hyperparameters
- threshold = 0.05
- n_clusters = 50
For this combination of hypereparameters, test_score is 0.6694 and train_score is 0.67877. So, model is not overfitted.

## Limitations and improvements possible
- We can experiment with different hyperparameters like `n_init` in KMeans, `hidden_layer_sizes`, `activation` and `max_iter` in `MLPClassifier`.
- But due limited computational power, we haven't tried them.
