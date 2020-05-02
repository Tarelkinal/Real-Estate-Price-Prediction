# Real-Estate-Price-Prediction
Solution for the Geekbrains AI/BigData Python for Data Science course competition https://www.kaggle.com/c/realestatepriceprediction

**EDA is implemented with Kaggle notebook in competition page https://www.kaggle.com/tarelkinal/eda-real-estate-price-prediction**

## Description
In this competition your task will be to predict the price of flats in test.csv. You will be given two datasets: train.csv (contains all features and prices of flats) and test.csv (only features).

## Evaluation
The evaluation metric is [Coefficient of determination](https://en.wikipedia.org/wiki/Coefficient_of_determination "Wikipedia") 

## Dataset description

### File descriptions

train.csv - the training set

test.csv - the test set

predictions.csv - file with answers in the correct format for submission 

### Data fields
Id - идентификационный номер квартиры

DistrictId - идентификационный номер района

Rooms - количество комнат

Square - площадь

LifeSquare - жилая площадь

KitchenSquare - площадь кухни

Floor - этаж

HouseFloor - количество этажей в доме

HouseYear - год постройки дома

Ecology_1, Ecology_2, Ecology_3 - экологические показатели местности

Social_1, Social_2, Social_3 - социальные показатели местности

Healthcare_1, Helthcare_2 - показатели местности, связанные с охраной здоровья

Shops_1, Shops_2 - показатели, связанные с наличием магазинов, торговых центров

Price - цена квартиры

## Solution
### [EDA](https://www.kaggle.com/tarelkinal/eda-real-estate-price-prediction "Kaggle notebook")
### Cleaning data
- Finding data outliers with EDA
- Using linear regression model for filling linear depending features (Square-LifeSquare, Square-KitchenSquare)
- Using medians by districts and global medians for Nans handling
### Feature endineering
- Categorical features embeddings
- Target encoding
### Model
- Gradient Boosting Machines
- train cv-score: **0.750 +- 0.018**
- 30% of sample test score: **0.75057**

