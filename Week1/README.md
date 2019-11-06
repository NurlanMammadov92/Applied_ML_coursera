# Assignment 1 - Introduction to Machine Learning


For this assignment, you will be using the Breast Cancer Wisconsin (Diagnostic) Database to create a classifier that can help diagnose patients. First, read through the description of the dataset (below).



## Question 0 (Example)

How many features does the breast cancer dataset have?

*This function should return an integer.*


## Question 1

Scikit-learn works with lists, numpy arrays, scipy-sparse matrices, and pandas DataFrames, so converting the dataset to a DataFrame is not necessary for training this model. Using a DataFrame does however help make many things easier such as munging data, so let's practice creating a classifier with a pandas DataFrame

Convert the sklearn.dataset cancer to a DataFrame.
*This function should return a (569, 31) DataFrame with*

*columns* =
['mean radius','mean texture','mean perimeter','mean area,
'mean concave points']

['mean radius', 'mean texture', 'mean perimeter', 'mean area',
'mean smoothness', 'mean compactness', 'mean concavity',

'mean concave points', 'mean symmetry', 'mean fractal dimension',

'radius error', 'texture error', 'perimeter error', 'area error',

'smoothness error', 'compactness error', 'concavity error',

'concave points error', 'symmetry error', 'fractal dimension error',

'worst radius', 'worst texture', 'worst perimeter', 'worst area',

'worst smoothness', 'worst compactness', 'worst concavity',

'worst concave points', 'worst symmetry', 'worst fractal dimension',

'target']

*and index* =

RangeIndex(start=0, stop=569, step=1)


## Question 2

What is the class distribution? (i.e. how many instances of malignant (encoded 0) and how many benign (encoded 1)?)

*This function should return a Series named target of length 2 with integer values and index = ['malignant', 'benign']*



















