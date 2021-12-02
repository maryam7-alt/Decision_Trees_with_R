# Decision_Trees_with_R 
#done by Meryem Jemaa

In this repository I will work on Simple and Advanced Decision Trees.

Simple Decision Trees: 
* Classification Trees 
* Regression Trees 
* Tree Pruning ( this is very important as it removes part of the tree that does not give any relevance to the classification). 

Advanced Decision Trees and boosting Techniiques: 
* Bagging or bootstrap aggregation ( to reduce variance within dataset) 
* Random Forest 
* Gradient Boosting (optimizer, minimize the error while using the loss function)
* ADA boost (stands for adaptive boosting : higher weights assigned to incorrectly classified instances)
* XG Boost (uses the 2nd derivative : a library for developing fast and high performance gradient boosting tree models)


Before we start the coding it is important to know why we classify and predict in the first place.
machine learning aims and attempt to find the relationship between input and output variables.
An analyst will use machine learning to price anything given historical variables for example. Y = f(V1, V2,V3...), f(x) defines the relationship between dependant variables and independant variables.

Why would we want to estimate F(x) : 

* we want to know the price of a given house, product, service
* we want to investigate the relationship between the output and the different input variables and that is what we can inferential statistiques. 

The choice we make will allow us to choose the model for estimating.
* In the prediction we make sure that the accuracy is optimal and the best among other models
* While inferencing we make sure that it explains the relationship and the statistical significance of the variables to the predicted function.

For example linear regression is simple to interpret, but sometimes it can't predict the y accurately.However, non-linear models may be predicting very accuartely and still the relationship can be difficult to understand.
After specifying the model now we want to concentrate on the type of learning : 
* *Parametric approach*: we assume the form of the realtionship ( example: linear) -- May not be as accurate as we want but we use it for inference
* *Non-Parametric approach* Here we don't assume any finctional form we just assume it through estimating and ploting the predicted output --needs a large amount of data and we 
use it for prediction mostly. 

We have two types of decision trees: 
* Regression Trees : for continous quantitative variable ( predicting revenue, marks,..)
* Classification Trees: For discrete categorical target variables ( Predicting high or low, win or loss, low risk/ high risk)
Terminologies: 
*Root node
*Splitting
*Decision node 
subtree
Leaf/Terminal node 


Recrusive binary splitting : 
* top down and greedy : it starts at the toop of the tree and then succesively splits the predictor space and greedy because at each step of the tree-building process, the best split is made at that particular step. 

#This is our Tree with package rpart: 

![image](https://user-images.githubusercontent.com/57539925/144463148-3d64d0b9-49c4-44ac-8c9d-13d32be45dc0.png) 

#Prediction on the Test Set: 

![image](https://user-images.githubusercontent.com/57539925/144509176-8d98ae65-e142-4d6d-a068-a5f071eb1bb3.png)

