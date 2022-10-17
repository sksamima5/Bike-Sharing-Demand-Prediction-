# Bike-Sharing-Demand-Prediction-
 Seoul Bike Sharing Demand Prediction



## Supervised ML- Regression model using Seoul Bike Sharing Demand Prediction Data Set


A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

Which variables are significant in predicting the demand for shared bikes. How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the Seoul based on some factors.






# Business Goal:


You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.



# Attribute Information:
## <b> Data Description </b>

### <b> The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.</b>


### <b>Attribute Information: </b>

* ### Date : year-month-day
* ### Rented Bike count - Count of bikes rented at each hour
* ### Hour - Hour of he day
* ### Temperature-Temperature in Celsius
* ### Humidity - %
* ### Windspeed - m/s
* ### Visibility - 10m
* ### Dew point temperature - Celsius
* ### Solar radiation - MJ/m2
* ### Rainfall - mm
* ### Snowfall - cm
* ### Seasons - Winter, Spring, Summer, Autumn
* ### Holiday - Holiday/No holiday
* ### Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

# Conclusions:
* #### As we have calculated MAE,MSE,RMSE and R2 score for each model. Based on r2 score will decide our model performance.
 

* ## Linear,Lasso,Ridge and ElasticNet.
* #### 1) Linear, Lasso, Ridge and Elastic regression models have almost similar R2 scores on both training and test data.(Even after using GridserachCV we have got similar results as of base models).

## Decision Tree Regressor:
 * #### On Decision tree regressor model, without hyperparameter tuning we got r2 score as 71% on training data and 68% on test data. Thus our model memorised the data.


## Random Forest:

 * #### On Random Forest regressor model, with hyperparameter tuning we got r2 score as 84% on training data and 81% on test data. Thus our model memorised the data.

## Gradient Boosting Regression(Gradient Boosting Machine):

* #### On Gradient Boosting Regression model, without hyperparameter tuning we got r2 score as 86% on training data and 85% on test data.Our model performed well without hyperparameter tuning.
* #### After hyperparameter tuning we got r2 score as 93% on training data and 91% on test data,thus we improved the model performance by hyperparameter tuning.

 **Thus Gradient Boosting Regression(GridSearchCV) and Random forest gives good r2 scores. We can deploy this models.**
