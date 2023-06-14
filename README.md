# Case-Study-on-KNN-Algorithm
KNN stands for K-Nearest Neighbour where K is hyper-parameter.
We are training a model using KNN Algorithm for the binary classification of the dataset. 
Here, we are performing KNN Algorithm on different types of datasets: UShaped, Concentric Circle, XOR and Linearly separable Dataset with different values of K, where K is the number of nearest neighbors.
As we know that in the KNN algorithm, unlike logistic regression we do not require a linear decision boundary to separate different classes of target variables.
So, this method produces a decision boundary that is not straight and has more scope than logistic regression.
KNN algorithm uses the Euclidian metric to quantify the nearness of data points, hence it is necessary to scale the dataset before performing the training.

After training the model, we cross-validate it on a cross-validation dataset by a method called, n-fold cross-validation to choose the best value of K. The K value corresponding to the highest value of the CV score is the best K value. This method is called the hyperparameter tuning process. Later we test the model on the test dataset and find out the evaluation metrics(usually accuracy and f1 score).

To sum it up, this is what is being done in the KNN algorithm.
  1) We assign a best value of K after the hyperparameter tuning process (K being the hyperparameter) to the model.
  2) For each new data point, from the Euclidean metric(distance), we locate k nearest neighbors.
  3) we assign the new data point to the class which is the class of the majority of KNN.

In our code, we have tried to perform KNN Algorithm on datasets with and without scaling the data to find out whether the K value(after hyperparameter tuning) is the same in both cases. It turns out that, K values in both cases may not be the same.

Similarly, we have also performed KNN Algorithm with n=5,10 ( n from n fold cross validation) to learn about the different results obtained from both the k values.
