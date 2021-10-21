# KC House Price Precition

# Abstract
This project aims to assist stakeholders, i.e. home buyers or real estate agents, in predicting the sale price of King county homes while demonstrating general trends in the market. Housing price trends are not only the concern of buyers and sellers, but it also indicates the current economic situation. This project uses an open source dataset, which include 20 explanatory features and 21,613 entries of housing sales in King County, USA. The paper involves predictions using various Regression techniques like linear regression, random forest regression, AdaBoostregression, and many others algorithms. Additionally, both feature engineering and feature reduction are performed throughout the analysis to reach to determine most effective model. This report suggests focusing the campaign on the following neighbourhoods: Medina, Clyde Hill and Mercer Island (the most expensive neighbourhoods). For the campaign we would recommend looking at houses with a grade of 10 or above. It also recommend launching the campaign in March/April,to gather interest with a view of completing the sale in Q2. Waterfront living is key, with the median house price for a house with a waterfront view being almost double that of one that does not have this feature. Lastly, The model provided gives more than 80% accuracy of the prices (80% of price variations explained by our model).



# Design
Online property companies offer valuations of houses using machine learning techniques. The aim of this report is to predict the house sales in King County, Washington State, USA using Multiple Linear Regression (MLR). Predicting house price accurately via machine learning models would enable government take action to ensure that companies don't manipulate the prices not to mention to ensure house prices are accessible to as many people as possible.

# Data
For this study, we collected data from the website named “Kaggle”-(https://www.kaggle.com/harlfoxem/housesalesprediction). Kaggle is a platform for predictive modelling and analytics competitions in which statisticians and data miners compete to produce the best models for predicting and describing the datasets uploaded by companies and users.

The dataset used in this project contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.The dataset consisted of 21 variables and 21613 observations.

# Algorithms

### Feature Engineering

1. Mapping Zipcode, latitide and longitude to create a new variable `Neighbourhoods` to provide more accurate results and prediction
2. Converting categorical features to binary dummy variables.
3. Extracting and adding two features, `monthly sales` and `quarterly sales` to explort the best time of the year to sell.

### Models
various Regression techniques like linear regression, random forest regression, AdaBoostregression, Decision tree are used to predict the house price. hyper-parameter is used in machine learning model to better guide the creation of the parameters which the models use to generate predictions on data. not to mention using cross validition in this part for more accurate results.

### Model Evaluation and Selection
evaluation metrics are a measure of how good a model performs and how well it approximates the relationship. we will consider the most famous metrics which are MSE, R-squared, and RMSE. The entire training dataset of 12,280 records is used to train the model which represent 60% of the date. 20% of the data is used to validate the training. Finally, Predictions on the 20% holdout were limited to the very end, so this split was only used and scores seen just once.

The official metric for DrivenData was R2(coefficient of determination); however, MSE and RMSE were included to provide a more useful real-world meaning.

#### Best Validation model is : 
with 94 features.

1. R-Square : 0.808
2. MSE : 7.01 e+9
3. RMSE : 83,729


#### Testing

1. R-Square : 0.799
2. MSE : 6.93 e+9
3. RMSE : 83,268

# Tools

* Numpy and Pandas for data manipulation.
* Scikit-learn for modeling.
* Matplotlib and Seaborn for plotting.
* Geopandas and geocoders to create maps and feature engineering.
* Bing API to obtain addresses.

# Communication

In addition to the slides and visuals presented. A website using Heroku will be provided for deployment. `Soon`

# Insights and Recommendations

1. Waterfront living is key, with the median house price for a house with a waterfront view being almost double that of one that does not have this feature.
2. following neighbourhoods: Medina, Clyde Hill and Bellevue (the most expensive neighbourhoods).
3. Location within King County is important with a noticeable disparity amongst zipcodes.
4. House prices do not appear to be affected by sale month or quarter, with the median house price being almost constant throughout the year.
5. April and May are the most popular months for sales. In contrast, January and February have the lowest sales. Q2 alone accounts for 31.3% of sales.



