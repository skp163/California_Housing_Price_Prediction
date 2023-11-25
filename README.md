# California Housing Price Prediction Using Different Models
## 1. Using Linear Regression
### About Data and Objective
This is an prediction project to predict median house values in Californian districts by given features in the data set.


**Data Set**:
[sklearn.datasets.fetch_california_housing](https://github.com/skp163/California_Housing_Price_Prediction/blob/main/Images/Feature%20Description.png)

**Number of Features : 8**
**Sample size: 20640**

## Process and Description
I have loaded the data and started with data understanding. 
Then I have converted the data set in to Pandas data frame for better visualisation. 
From here, I have check for data quality and  consistency.
Also I find the scaling of the features are not consistent. 2 features are capped features.  Target and HouseAge is caped by 0 to 5 and 0 to 52 respectively. This needed data preprocessing.

![Features Description](https://github.com/skp163/California_Housing_Price_Prediction/blob/main/Images/Feature%20Description.png)


Then I jump to feature selection and try to correlate each features with each other.

![Features Correlation](https://github.com/skp163/California_Housing_Price_Prediction/blob/main/Images/Features%20Correlation.png)



I find Median_Income is highly correlated with House_value than other features.

![Median_Income is highly correlated with house price](https://github.com/skp163/California_Housing_Price_Prediction/blob/main/Images/Housing%20price%20by%20Income.png)



Then I took general hypothesis as 'the price of any house is highly dependent on location' and find my hypothesis is right. At some special latitude -longitude the prices of the houses are very high.

![Location Vs Housing Price](https://github.com/skp163/California_Housing_Price_Prediction/blob/main/Images/HousingPrice%20By%20Loc.png)


Then I have done a simple linear regression including all the features and find the below results for R2 err and MSE. 

Result
-----

|R2_Error|  MSE  |
|--------|-------|
| 0.594  | 0.5424|

## Way Forword
Next to make it better, it needs extensive feature selection and data pre-processing.


