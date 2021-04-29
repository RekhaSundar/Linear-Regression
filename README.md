# Linear-Regression
Python 3 program

A program that implements a (batch) linear regression using the gradient descent method using the following gradient calculation:

<img width="246" alt="Formula" src="https://user-images.githubusercontent.com/56769691/116580015-98ae0d80-a930-11eb-9b8e-e979fc37e8f1.png">

where xi is one data point (with N being the size of the data set), η the learning rate, yi is the target output and f(xi) is the linear function defined as f(x) = transpose(w)* x or equivalently f(x) = Σwi · xi. Whereas w and x include the bias/intercept, i.e. w0 (x0 is always 1). All weights  initialized as 0. Given are the two random example data sets  named random1 and random2 as csv files. Using those data sets, the task is to correctly implement the gradient descent method and return for each iteration the weights and sum of squared errors until a given threshold of change in the error is reached.

The output looks like: 
iteration_number,weight0,weight1,weight2,...,weightN,sum_of_squared_errors

The solution is rounded to 4 decimals and for the data sets are given with a learning rate of 0.0001 and a threshold of 0.0001. Program accepts the following parameters:

1. threshold - The threshold, that the change in error has to fall below, before the algorithm terminates.
2. data - The location of the data file (e.g. /media/data/yacht.csv).
3. eta - The learning rate of the gradient descent approach.

