# Project Title : Bike_Sharing_Demand_Prediction_Capstone_Project

# Problem Description:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

# Steps Involved
* Importing libraries
* Exploratory Data Analysis
* Extracting features from date
* Model Building
1. Linear Regression
2. Lasso Regression
3. Ridge Regression
4. ElasticNet Regression
5. DecisionTree Regressor
6. RandomForest Regressor
7. Gradient Boost
8. Xg Boost
* Model Evaluation through Metrics :
1. Mena Squared Error
2. Root Mean Squared Error
3. R-Squared
4. Adjusted R-Squared
 
# Model Summary
+-------+------------------------+--------------------+--------------------+--------------------+--------------------+
| SL NO |       MODEL_NAME       |      Test MSE      |     Test RMSE      |      Test R^2      | Test Adjusted R^2  |
+-------+------------------------+--------------------+--------------------+--------------------+--------------------+
|   1   |   Linear Regression    | 50.71126097463167  | 7.121183958769192  | 0.6710932500851713 | 0.668060104264631  |
|   2   |    Lasso Regression    | 50.71557738931464  | 7.121487020932822  | 0.6710652543718449 | 0.6680318503775795 |
|   3   |    Ridge Regression    | 50.711251168967785 | 7.1211832702836535 | 0.6710933136834525 | 0.6680601684494094 |
|   4   | ElasticNet Regression  | 50.71147206222219  | 7.121198779855972  | 0.6710918809980688 | 0.6680587225519415 |
|   5   | DecisionTree Regressor | 28.74204997012355  | 5.361161252016539  | 0.8135827415868828 | 0.811863619895465  |
|   6   | RandomForest Regressor | 13.543575525802646 | 3.6801597147138394 | 0.9121581021097825 | 0.9113480327344261 |
|   7   |     Gradient Boost     | 13.48411102400463  | 3.6720717618266434 | 0.9125437812596556 | 0.9117372685796294 |
|   8   |        Xg Boost        | 19.37511776720657  | 4.401717592850156  | 0.8743354653078561 | 0.8731765992818767 |
+-------+------------------------+--------------------+--------------------+--------------------+--------------------+

# Conclusions:

* As it was stated in the problem, rented bike count was low in 2017 untill november. After that rented bike count started increasing.
* There was sharp increase in demand from the end of 2017 that too in winter season of the year. The demand however decrease at the end of 2018.
* Bike count rent is highly correlated with 'Hour', which seems obvious. Demand for bike is mostly in morning (7 to 8) and in the evening (3 to 9).
* After doing exploratory data analysis, applying Linear Regression model didn't go quite well as it gave only 67.109325% accuracy.
* Lasso and Ridge Regression helps to reduce model complexity and prevent over-fitting which may result from simple linear regression. with Lasso, ridge and ElsasticNet regressor We got r squared value of 0.67106525, 0.67109331, 0.67109188 respectively.
* With Decision Tree we are able to achieve the r2 score of 0.811.
* Random forest regressor gave r squared value of 0.911 on test data.
* Gradient Boost gives higher value of R squared metric in train data 0.947 and on test data it is 0.912
* XG Boost gave r squared value of 0.874
* Gradient Boost came with best accuracy to approximate numbers of rented bikes demand. It gives amazing results of training r-square at 0.94 and test r-square value at 0.912 also with adjusted r-square with 0.911.

