# Data-Scaling
Explaining how Data Scaling increases the accuracy of the model and reduces bias.

Standardization is a preprocessing method used to transform continuous data to make it look normally distributed. In scikit-learn this is often a necessary step because many models assume that the data you are training on is normally distributed, and if it isn't, your risk biasing your model.

It’s also important to note that *standardization* is a preprocessing method applied to continuous, numerical data, and there are a few different scenarios in which you want to use it:

1. When working with any kind of model that uses a linear distance metric or operates on a linear space — KNN, linear regression, K-means
2. When a feature or features in your dataset have high variance — this could bias a model that assumes the data is normally distributed, if a feature in has a variance that’s an order of magnitude or greater than other features
