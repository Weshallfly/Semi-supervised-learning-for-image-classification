# Semi-superwised-learning-for-image-classification
This repository contains an implementation of semi-supervised learning using K-Means clustering on the Fashion MNIST.

## Datasets
Fashion MNIST: A dataset of Zalando's article images consisting of 60,000 training images and 10,000 testing images, with 10 classes.

## Prerequisites
- Python 3.7+
- Required libraries: numpy, pandas, scikit-learn, tensorflow or keras, matplotlib

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

## Conclusion
This experiment demonstrates the effectiveness of using K-Means clustering for semi-supervised learning on the Fashion MNIST dataset. By leveraging clustering, we can significantly reduce the amount of labeled data needed for training while maintaining high classification performance.

## Limitations and improvements possible
- We can experiment with different hyperparameters like `n_init` in KMeans, `hidden_layer_sizes`, `activation` and `max_iter` in `MLPClassifier`.
- But due limited computational power, we haven't tried them.
