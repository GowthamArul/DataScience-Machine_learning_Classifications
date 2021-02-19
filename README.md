# DataScience-Machine_learning_Classifications


## Logistic Regression
=======================
INTUITION

*) Logistic regression algorithm works by implementing a linear equation first with independent predictors to predict value.
*) We then need to convert this value into a probability that could range from 0 to 1
*) From Probability To Class: Now we need to convert from a probability to a class value which is "0" or "1"

# Linear equation
================

y = b0 + b1 * x

apply sigmoid function
----------------------

p(x) = sigmoid(y)
p(x) = 1/1+e^-y
p(x) = 1/1+e^-(b0+b1*x)

# K-Nearest Neighbors
====================
INTUITION

*) K-Nearest Neighbors algorithm (KNN) is a classification algorithm.
*) KNN works by finding the most similar data points in the training data, and attempt to make an educated guess based on their classifications. 

Algorithm Steps
---------------

1) Select a value for k (e.g.: 1, 2, 3, 10..)
2) Calculate the Euclidian distance between the point to be classified and every other point in the training data-set
3) Pick the k closest data points (points with the k smallest distances)
4) Run a majority vote among selected data points, the dominating classification is the winner! Point is classified based on the dominant class.
5) Repeat!

𝑬𝒖𝒄𝒍𝒊𝒅𝒆𝒂𝒏 𝑫𝒊𝒔𝒕𝒂𝒏𝒄𝒆= √((𝒙_𝟐−𝒙_𝟏 )^𝟐+(𝒚_𝟐−𝒚_𝟏 )^𝟐 )

#  Decision Trees
===============
INTUITION

*) Decision Trees are supervised Machine Learning technique where the data is split according to a certain condition/parameter. 
*) Let’s assume we want to classify whether a customer could retire or not based on their savings and age.

DEFINITIONS

*) The tree consists of decision nodes and leaves. 
*) Leaves are the decisions or the final outcomes.
*) Decision nodes are where the data is split based on a certain attribute.
*) Objective is to minimize the entropy which provides the optimum split 

# RANDOM FOREST
================
INTUITION

*) Random Forest Classifier is a type of ensemble algorithm. 
*) It creates a set of decision trees from randomly selected subset of training set. 
*) It then combines votes from different decision trees to decide the final class of the test object.

WHY AND HOW?

*) It overcomes the issues with single decision trees by reducing the effect of noise.
*) Overcomes overfitting problem by taking average of all the predictions, canceling out biases.
*) Suppose training set: [X1, X2, X3, X4] with labels: [L1, L2, L3, L4]
*) Random forest creates three decision trees taking inputs as follows:
   [X1, X2, X3], [X1, X2, X4], [X2, X3, X4]
*) Example: Combining votes from a pool of experts, each will bring their own experience and background to solve the problem resulting in a better outcome. 
