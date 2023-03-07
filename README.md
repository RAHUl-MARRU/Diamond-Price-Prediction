# Diamond-Price-Prediction
Advance Statistical Learning - R Programming Language Code

# Abstract: 


Gemstones like diamonds are always in demand because of their value in the investment market. 
This makes it very important for diamond dealers to predict its accurate price. However, the 
prediction process is difficult due to the wide variation in the diamond stones sizes and 
characteristics [1]. We are solved the problem of predicting diamond prices in the United States 
by Subset Selection and Shrinkage Methods like Forward selection, Backward selection, LASSO
and Ridge Regression models.

# Dataset Source: 

The data is collected from the data.world, It consists of the number of 
observations are 53940(almost 54000) and the number of predictors is 11.

# Link: https://data.world/nahrin/diamonds

# Dataset Description

Attribute Description

price in US dollars ($326 - $18,823)

carat weight of the diamond (0.2 - 5.01)

cut quality of the cut (Fair, Good, Very Good, Premium, Ideal)

color diamond color, from J (worst) to D (best)

clarity a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, 
VS1, VVS2, VVS1, IF (best))

X length in mm (0 - 10.74)

y width in mm (0 - 58.9)

z depth in mm (0 - 31.8)

depth total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43 - 79)

table width of top of diamond relative to widest point (43 - 95)

# Step-By-Step’s in work approach

• Import required libraries.

• Data Preprocessing/Feature Engineering and EDA.

• FEATURE SELECTION {Train-Test-Split}

• Model Building And 

• Evaluation.

# Modeling Techniques


Stepwise Selection -> Forward selection,  Backward selection.

 Lasso Regression
 
 Ridge Regression
 
 # Metrics for Evaluating Regression Model Performance:
 
 Root Mean Square Error
 
 ![image](https://user-images.githubusercontent.com/125625532/223500350-504c7226-ac24-4931-9acf-cb24eca6a07f.png)

Coefficient of Determination or R^2

![image](https://user-images.githubusercontent.com/125625532/223500504-46e529d3-cc83-4a0b-85cc-a66d483fb207.png)

# Mean Square Error Comparison on Lasso and Ridge Regression

![image](https://user-images.githubusercontent.com/125625532/223501032-8f0e9dc3-4003-4842-a56e-c514b544a956.png)

![image](https://user-images.githubusercontent.com/125625532/223501118-5434d7d6-ba97-4c29-8be2-ec24da1cca4b.png)


 
 # Conclusion
 
 By comparing Lasso regression or L1 Regularization got better than Ridge Regression models
when we compared in Plot. The amount of shrinkage for each method is determined by lambda, a 
tuning parameter. Lambda was chosen for each method by 10-fold cross validation using the 
mean squared error on the training set to measure performance. The optimal lambda for ridge 
regression is 367.57 and optimal lambda for lasso model is 2.1588. Lasso is a more 
accurate model compared to ridge regression.
When comparing all the four techniques such as Forward Selection, Backward Selection, Lasso 
and Ridge Regression. Among these both forward selection and backward selection got best R-squared score – 0.9198 than other models. 
We can reduce the score of MSE of each by normalize the data. Due the response values are 
much long range in between other predictors.




