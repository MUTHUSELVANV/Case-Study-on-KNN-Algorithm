# Case-Study-on-KNN-Algorithm
KNN stands for K-Nearest Neighbour where K is hyper-parameter
We are training a model using KNN Algorithm for binary classification of the dataset. 
Here, we are performing KNN Algorithm on different types of dataset: UShaped, Concentric Circle, XOR and Linearly separable Dataset with different values of K, where K in number of nearest neighbor.
As we know that in KNN algorithm, unlike logistic regression we do not require a linear decision boundary top seperate different classes of target variables.
So, this method produces decision boundary that is not straight and has more sccope than logistic regression.
KNN algorithm uses eucledian metric to quantify the nearness of datapoints, hence it is recessary to scale the dataset before performing the training.

After training the model, we cross validate it on cross validation dataset by a method called, n-fold cross validation to choose the best value of K. The K value corresponding to the highest value of CV score is the best K value. This method is called hyperparameter tuning process. Later we test the model on the test dataset and find out the evaluation metrics(usually accuracy and f1 score).

To sum it up, this is what is being done in KNN algorithm.
  1) We assign a best value of K after hyperparameter tuning process (K being the hyperparameter) to the model
  2) For each new datapoint, from the eucledian metric(distance), we locate k nearest neighbours
  3) we assign the new datapoint the class which is the class of majority of KNN.

In our code, we have tried to perform KNN Algorithm on datasets with and without scaling the data to find out whether K value(after hyperparameter tuning) is same in both the cases. It turns out that, K values in both the cases may not be same.

Similary, we have also performed KNN Algorithm with n=5,10 ( n from n fold cross validation) to learn about the different results obtained from both the k values.
