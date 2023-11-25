# California Housing Price Prediction Using Different Models
## 1. Using Linear Regression
### About Data and Objective
This is an prediction project to predict median house values in Californian districts by given features in the data set.


**Data Set**:
[sklearn.datasets.fetch_california_housing](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)


## Process and Description
I have loaded the data and started with data understanding. 
Then I have converted the data set in to Pandas data frame for better visualisation. 
From here, I have check for data quality and  consistency.
Also I find the scaling of the features are not consistent. 2 features are capped features.  Target and HouseAge is caped by 0 to 5 and 0 to 52 respectively. This needed data preprocessing.

Image

Then I jump to feature selection and try to correlate each attributes with each other. I find Median_Income is highly correlated with target(House_value) than other features.
Then I took general hypothesis as 'the price of any house is highly dependent on location' and find the it right. At some latitude -longitude the prices of the house is very high. 
Then I have done a simple linear regression including all the features and find the below results for R2 err and MSE. 

Result
-----

|R2_Error|  MSE  |
|--------|-------|
| 0.594  | 0.5424|

## Way Forword
Next to make it better, it needs extensive feature selection and data pre-processing.


