# kaggle_cardekho

## Problem Statement
CarDekho.com is India's leading car search venture that helps users buy cars that are right for them. 
Its website and app carry rich automotive content such as expert reviews, detailed specs and prices, 
comparisons as well as videos and pictures of all car brands and models available in India. 

The kaggle competiton is to predict the car price using the set of features provided for each car.

## Correlation heatmap 

![alt text](https://github.com/SHINE1607/kaggle_cardekho/blob/master/images/correlation_heatmap.png)

## scattered Correlation between variables

![alt text](https://github.com/SHINE1607/kaggle_cardekho/blob/master/images/correlation.png)

## features with most correlation with target variable

![alt text](https://github.com/SHINE1607/kaggle_cardekho/blob/master/images/feature_importance.png)

## Model used 

From the correlation heat map and scatter plot we can see that the variables have strong correlation
with the target variable and the non-linearity in the model is substantially more.
therefore I used Random forest regressor and tuned using RandomizedSearchCV and bet parameters turned out 
to be :
{'n_estimators': 700,
  'min_samples_split': 15,
  'min_samples_leaf': 1,
  'max_features': 'auto',
  'max_depth': 20}

## Prediction distplot

Distplot of predicted_value - actual_value
![alt text](https://github.com/SHINE1607/kaggle_cardekho/blob/master/images/prediction.png)
We can see that distribution has a peak at 0, showing a good prediction in values

## Evaluation
mean absolute error: 0.8701179228754423
mean squares error: 2.631077516024701

