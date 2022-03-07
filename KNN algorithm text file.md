K-Nearest Neighbour(KNN) Algorithm for Machine Learning.

K-Nearest Neighbour is one of the simplest machine learning algorithms based on
supervised learning technqiue.

K-NN algorithm assumes the similarity between the new case/data and available cases
and put the new case into the category that is most similar to the available 
categories.

K-NN algorithm stores all the available data and classifies a new data point based on
the similarit. This means when new data appears then it can be easily classified into
a well suite category by using the k-NN algorithm.

K-NN algorithm can be used for regression as well as for the Classification but mostly it is
used for the classification problems

K-NN is a non-parametric algorithm, which means it does not make any assumption on underlying data.

It is also  called a lazy learner algorithm because it does not learn from the training
set immediately instead it stores the dataset and at the time of classification, it performs
an action on the dataset.

K-NN algorithm at the training phase just stores the dataset and when it gets new data,
then it classifies  that data into a category that is muh similar to the new data..

EG: Suppose, we have an image of a creature that looks similar to cat and dog,
    but we want to know either it is a cat or dog. So for this identification, we can use
    the KNN algorithm, as it works on a similarity measure. Our KNN model will find the 
    similar features of the new data set to the cats and dogs images and based on the most
    similar features it will put it in either cat or dog category.
    
    
Why do we need a K-NN algorithm?

Suppose there are two categories,i.e, category A and B, and we have a new data points
x1, so this data point will lie in which of these categories. To solve this type
of problem, we need a K-NN algorithm. With the help of K-NN, we can easily identify
the category or class of a particular dataset. Consider the below diagram.

How does K-NN work?
The K-NN working can be explained on the basis of the below diagram.

step 1: Select the number K of the neighbors
step 2: Calculate the Euclidean distance of K number of neighbors
step 3: Take the K nearest neighbors as per the calculated Euclidean distance.
step 4: Among these k neighbors, count the number of the data points in each category
step 5: Assign the new data points to that category for which the number of the neighbor is maximum.
Step 6: Out model is ready

Suppose we have a new data point and we need to put it in the required category.
Consider the below image:
    
Firstly, we will choose the number of neighbours, so we will choose the k=5
Next, we will calculate the Euclidean distance between the data points. The Euclidean
distance is the distance between the two points, which we have already studied in
geometry. It can be calculated as:
    
By calculating the Euclidean distance we got the nearest neighbors, as three nearest
neighbors in category A and two nearest neighbours in category B. Consider the below
image:
    
    
As we can see the 3 nearest neighbours are from the category A, hence this new data point
must be belong to category A.

How to select the value of K in the K-NN Algorithm

Below are some points to remember while selecting the value of k in the K-NN
algorithm:
    
There is no particular way to determine the best value for "K", so we need to try
some values to find the best out of them. The most perferred value for K is 5..
A very low value for K such as K=1, K=2, can be noisy and lead to the effects of
outliers in the model.

Large values for K are good, but it may find some difficulties.

Advantages of KNN Algorithm:
    
    1.It is simple to implement.
    2.It is robust to the noisy training data.
    3.It can be more effective if the training data is large.
    
Disadvantages of KNN Algorithm:
    1. Always needs to determine the value of K which may be complex some time.
    2. The computation cost is high because of the calculating the distance betwen the data
    points for all training samples.
    
    
Python implementation of KNN algorithm:   
    
To do the python implementation of KNN algorithm, we will use the same problem and 
dataset which we have used in the logistic regression. But here we will improve the
performance of the model. Below is the problem description:
    
    
Problem for K-NN Algorithm: There is a car manufacturer company that has manufactured
    a new SUV car. The company wants to give the ads to the users who are interested in
    buying that SUV. So for this problem, we have a dataset that contains multiple users
    information through the social network. The dataset contains lots of information but
    the Estimated Salary and Age will consider for the independent variables and the
    Purchased variables is for the dependent variable. Below is the dataset:
        
        
Steps to implementation of K-NN Algorithm:
    
    
1. Data Pre-processing step
2. Fitting the K-NN algorithm to the training set.
3. Predicting the test result.
4. Test accuracy of the result(Creation of Confusion matrix)
5. Visualizing the test set results.

Data Pre-Processing Step:

The Data Pre-processing step will remain exactly the same as Logistic Regression. 
Below is the code for it:    