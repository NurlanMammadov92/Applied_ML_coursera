
# Assignment 3 - Evaluation

In this assignment you will train several models and evaluate how effectively they predict instances of fraud using data based on [this dataset from Kaggle](https://www.kaggle.com/dalpozz/creditcardfraud).

Each row in `fraud_data.csv` corresponds to a credit card transaction. Features include confidential variables V1 through V28 as well as Amount which is the amount of the transaction.

The target is stored in the `class` column, where a value of 1 corresponds to an instance of fraud and 0 corresponds to an instance of not fraud.


## Question 1

Import the data from `fraud_data.csv`. What percentage of the observations in the dataset are instances of fraud?

*This function should return a float between 0 and 1.*

## Question 2

Using `X_train`,`X_test`,`y_train`, and `y_test` (as defined above), train a dummy classifier that classifies everything as the majority class of the training data. What is the accuracy of this classifier? What is the recall?

*This function should a return a tuple with two floats, i.e. (accuracy score, recall score).*

## Question 3

Using `X_train`,`X_test`,`y_train`,`y_test` (as defined above), train a SVC classifer using the default parameters. What is the accuracy, recall, and precision of this classifier?

*This function should a return a tuple with three floats, i.e. (accuracy score, recall score, precision score).*


## Question 4


Using the SVC classifier with parameters {'C': 1e9, 'gamma': 1e-07}, what is the confusion matrix when using a threshold of -220 on the decision function. Use `X_test` and `y_test`.

*This function should return a confusion matrix, a 2x2 numpy array with 4 integers.*


## Question 5

Train a logisitic regression classifier with default parameters using `X_train` and `y_train`.

For the logisitic regression classifier, create a precision recall curve and a roc curve using `y_test` and the probability estimates for `X_test` (probability it is fraud).

Looking at the precision recall curve, what is the recall when the precision is 0.75?

Looking at the roc curve, what is the true positive rate when the false positive rate is 0.16?

*This function should return a tuple with two floats, i.e. (recall, true positive rate).*



## Question 6


Perform a grid search over the parameters listed below for a Logisitic Regression classifier, using recall for scoring and the default 3-fold cross validation.

'penalty': ['l1', 'l2']

'C':[0.01, 0.1, 1, 10, 100]

From `.cv_results_`, create an array of the mean test scores of each parameter combination. i.e.

|      |**l1** |**l2**|
| -- |:-------------:| -----:|
|0.01| ? | ?|
|0.1|?|?|
|1|? |? |
|10|? |? |
|100|? |? |






















