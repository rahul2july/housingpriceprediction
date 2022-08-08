# Project Name: Housing Price Prediction
### Business Objective
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
##### Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
-Which variables are significant in predicting the price of a house, and
-How well those variables describe the price of a house.
-Also, determine the optimal value of lambda for ridge and lasso regression.

We are required to model the price of houses with the available independent variables. 
This model will then be used by the management to understand how exactly the prices vary with the variables. 
They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. 
Further, the model will be a good way for management to understand the pricing dynamics of a new market.

Dateset could be found here: https://github.com/rahul2july/housingpriceprediction/blob/main/data_description.txt

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- In summary, for ridge: <br>
-the best hyperparameter alpha is 7.0 <br>
-r-squared train = 0.8507, r-squared test: 0.8545 <br>
-There is slight improvement in r-squared test when compared to linear regression. <br>
-Top 5 features defining "SalePrice" are: <br>
    -Fence_GdWo <br>
    -GarageType_N.A <br>
    -YearBuilt_diff <br>
    -OverallCond <br>
    -LotFrontage <br>
    
- In summary, for lasso: <br>
-the best hyperparameter alpha is 0.001 <br>
-r-squared train = 0.8512, r-squared test: 0.8533 <br>
-There is slight improvement in r-squared test when compared to linear regression. <br>
-Top 5 features defining "SalePrice" are: <br>
    -Fence_GdWo <br>
    -GarageType_N.A. <br>
    -YearBuilt_diff <br>
    -OverallCond <br>
    -LotFrontage <br>
    
- RSS is very close for all the three models [linear regression, ridge regression and lasso regression]. <br>
We could see that Lasso seems to be performing a little better out of the three models wrt. mse. <br>
Since Lasso will penalize more on the dataset and can also help in feature elimination hence we are going to consider that as my final model. <br>

- Looking at the coefficients, we could conclude that features like: <br>
OverallQual, GrLivArea, SaleType_New etc. have a positive impact on SalePrice. <br>
BldgType_Twnhs, BldgType_Duplex, Condition1_PosN have a negative impact on SalePrice. <br>

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used 
-python - version 3.9.13 <br>
-numpy - version 1.22.2 <br>
-pandas - version 1.4.1 <br>
-matplotlib - version 3.5.1 <br>
-seaborn - version 0.11.2 <br>
-sklearn - version 1.1.1 <br>
-statsmodels - version 0.13.2 <br>

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project was inspired by Linear Regression Assignment as part of Data Science course. <br>
This project was based on: https://learn.upgrad.com/course/1991/segment/25160/150983/463809/2405074

## Contact
Created by [@rahul2july] - feel free to contact me! <br>

Contributor -Rahul Gupta


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->