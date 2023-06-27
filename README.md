# Project Name
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.
 
The company wants to know:

#Which variables are significant in predicting the price of a house, and

#How well those variables describe the price of a house.

 
Also, determine the optimal value of lambda for ridge and lasso regression.


Business Goal 

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

# General Information

- Given dataset train.csv file has about 81 columns including id columns
- Performed EDA on given data set
	- Identified that NaN values may have some impact on Sales Price
	- Identified that Month Sold has no impact on the price
	- Prepared new columns like age, garage_agem remodel_age
	- Dropped 'GarageYrBlt'
	- had to convert a few columns to string, not to treat them as numerical
	- identified a few columns like 'Street', 'Utilities', 'PoolArea', 'PoolQC' have about 99% same values, hence dropped them
	
# Conclusions

- We are able to achieve an R2 score of 0.82 approx on both Ridge and Lasso Models. 

- Following factors influence the house price the most as demonstrated by both models:-
    - Total area in square foot
    - Total Garage Area
    - Total Rooms
    - Overall Condition
    - Lot Area
    - Centrally Air Conditioned
    - Total Porch Area (Open + Enclosed)
    - Kitchen Quality
    - Basement Quality
