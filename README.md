
This repository presents an implementation of the Anomaly Detection Algorithm using Gaussian Mixture Model (GMM) for credit card fraud detection. The dataset contains credit card transactions, categorized as fraudulent or non-fraudulent, and includes features such as transaction amount, time, and transaction type.

To facilitate model development, the dataset is split into training, validation, and test sets. The training set is utilized for model training, the validation set aids in hyperparameter tuning, and the test set evaluates the final model's performance.

In the exploratory data analysis (EDA) phase, we investigate the distribution differences for selected variables between fraudulent and non-fraudulent transactions. This examination helps discern the distinguishing characteristics between the two types of transactions.

Several models are implemented and evaluated:

One Gaussian Model with Single Feature: This model fits a single Gaussian distribution to each individual feature, assuming a unimodal Gaussian distribution.

One Gaussian Model with Multiple Features: Similar to the previous model, but considering multiple features simultaneously.

Two Gaussian Model with Single Feature: Here, the data is assumed to follow a bimodal Gaussian distribution, with separate Gaussian distributions for fraudulent and non-fraudulent transactions.

Multivariate Gaussian Distribution: This model captures correlations between multiple features by modeling the joint distribution using a multivariate Gaussian distribution.

Mixture of Gaussians Distribution: Using a mixture of Gaussian distributions, this model can capture more complex patterns and distributions in the data.

Model evaluation is conducted on the test data, employing metrics such as accuracy, precision, recall, and F1 score. The model exhibiting the highest performance, in terms of accurately identifying fraudulent transactions while minimizing false positives, is selected as the best-performing model.
