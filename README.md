# FYS-STK4155 - Applied statistics and machine learning
In this course we focus on how machine learning can be used in real-world applications, in particular how we can fit a model to real terrain data (Project 1) and how we can determine the energy and phase of the two-dimensional Ising model. In a third project, we..

## Project 1
The aim of this project is to study the performance of linear regression in order to fit a two dimensional polynomial to terrain data. Both Ordinary Least Square (OLS), Ridge and Lasso regression methods were implemented, and for minimizing Lasso’s cost function Gradient Descent (GD) was used. A fourth method was to minimize the cost function of Ridge using GD. The fitted polynomial was visualized and compared with the data, the Mean Square Error (MSE) and R2-score were analyzed, and finally the polynomial coefficients were studied applying visualization tools and Confidence Intervals (CI). To benchmark the results, we used Scikit Learn. 

We found the self-implemented OLS and Ridge regression functions to reproduce the benchmarks, and Lasso was close to reproducing the benchmark as well. However, the difference between results produced by standard Ridge regression and when minimizing its cost function is large. The OLS regression method is considered as the most successful due to its small MSE and high R2-score.


## Project 2
In this project we first determine the energy in the one-dimensional Ising model using linear regression and deep learning. We will investigate the performance of both Ordinary Least Square (OLS), Ridge regression and Lasso regression, before we turn to a deep feed-forward neural network (FNN) with various activation functions and hyper parameters. Secondly, we classify the phase of a two-dimensional Ising model using logistic regression and deep learning, and vary the regularization parameter.

To estimate the error, Mean Square Error (MSE) and the R$^2$-score function are used in the regression case, and we find more reliable values by K-fold validation resampling. In the classification case, we will study the accuracy score since the outputs are binary. Gradient descent (GD) and stochastic gradient descent (SGD) are implemented as the minimization tools. 

In linear regression, Lasso and Ridge regression gave smaller MSE (below $10^{-4}$) compared to OLS, and only Lasso was able to recall the correct J-matrix. Using a neural network, a pure linear activation function on a hidden layer gave best results. For classification, logistic regression did not work well, but with a neural network we were able to obtain an accuracy above 99\% for a test set far from the critical temperature and above 96\% for a test set close to the critical temperature using three hidden layers with \textit{Rectified Linear Units} (ReLU) and \textit{leaky} ReLU activation functions.

## Project 3
