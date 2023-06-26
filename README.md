# tehran-house-price-prediction
# House Price Prediction using Tehran Housing Data

This project aims to predict house prices in Tehran using real housing data. 

## The Dataset

The dataset consists of information for approximately 4000 apartments in Tehran. All data is real. The task is to predict the price in dollars or rials using the features provided:

- Area: Area in meters  
- Room: Number of bedrooms
- Parking: If parking is available or not 
- Warehouse: If warehouse is available or not
- Elevator: If elevator is available or not
- Address: Approximate address in Tehran  
- Price: Price in Iranian rials
- Price(USD): Price in US dollars

Some houses have missing address data and some have incorrect area values (very large). These should be removed from the dataset.

## Data Preprocessing and Feature Engineering

The data will be cleaned by:

- Removing records with missing address 
- Removing records with area over 1000 square meters
- Encoding categorical variables (parking, warehouse, elevator) as dummy variables
- Scaling input features 

Features like number of floors, age of building, etc. could also be engineered from the address.

## Modelling

Several machine learning models will be trained and compared:

- Linear Regression   
- Random Forest   
- Neural Network

Models will be evaluated using:

- Mean Absolute Error 
- Mean Squared Error

The best model will be selected based on accuracy on a held-out test set.

## Potential to Improve

The model could be improved by:

- Obtaining a larger dataset 
- Incorporating more relevant features 
- Trying more advanced algorithms like XGBoost    

Overall, this project demonstrates an approach to predicting house prices in Tehran using real housing data and machine learning techniques. By expanding the dataset and optimizing the model, more accurate predictions could be achieved.
