# IRIS FLOWER DATASET

### SUMMARY OF WHAT I HAVE DONE IN THIS LEARNING NOTEBOOK

#### (Source: 'Introduction to Machine Learning using Python' by Andreas C. Müller & Sarah Guido)

The Iris dataset consists of two NumPy arrays: one containing the data, which is
referred to as X in scikit-learn , and one containing the correct or desired outputs,
which is called y . The array X is a two-dimensional array of features, with one row per
data point and one column per feature. The array y is a one-dimensional array, which
here contains one class label, an integer ranging from 0 to 2, for each of the samples.

We split our dataset into a training set, to build our model, and a test set, to evaluate
how well our model will generalize to new, previously unseen data.

We chose the k-nearest neighbors classification algorithm, which makes predictions
for a new data point by considering its closest neighbor(s) in the training set. This is
implemented in the KNeighborsClassifier class, which contains the algorithm that
builds the model as well as the algorithm that makes a prediction using the model.
We instantiated the class, setting parameters. Then we built the model by calling the
fit method, passing the training data ( X_train ) and training outputs ( y_train ) as
parameters. We evaluated the model using the score method, which computes the
accuracy of the model. We applied the score method to the test set data and the test
set labels and found that our model is about 97% accurate, meaning it is correct 97%
of the time on the test set.

This gave us the confidence to apply the model to new data (in our example, new
flower measurements) and trust that the model will be correct about 97% of the time.
