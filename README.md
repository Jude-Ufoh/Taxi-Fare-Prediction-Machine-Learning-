# Taxi-Fare-Prediction-Machine-Learning-
# About the Project
This is a supervised machine learning regression problem. It involves the  training of  a machine learning model to predict the fare for a taxi ride in New York city given information like pickup date & time, pickup location, drop location and no. of passengers.

# Data Source
The data was sourced from kaggle [link](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/overview)
### Features
- pickup_datetime - timestamp value indicating when the taxi ride started.
- pickup_longitude - float for longitude coordinate of where the taxi ride started.
- pickup_latitude - float for latitude coordinate of where the taxi ride started.
- dropoff_longitude - float for longitude coordinate of where the taxi ride ended.
- dropoff_latitude - float for latitude coordinate of where the taxi ride ended.
- passenger_count - integer indicating the number of passengers in the taxi ride.
### Target
- fare_amount - float dollar amount of the cost of the taxi ride.
  
# Task
The task is to build a machine learning model that will be evaluated on the basis of Root Mean Square Error (RMSE).
RMSE measures the difference between the predictions of a model, and the corresponding ground truth. A large RMSE is equivalent to a large average error, so smaller values of RMSE are better. 

# Procedure
**Download the Dataset**
- Install Required Libraries
- Download Data from Kaggle
- View Dataset Files
- Loading Training Set
- Load Test Set
  
**Explore the Dataset**
- Training Set
- Test Set
- Exploratory Data Analysis and Visualization
  
**Prepare Dataset for Training**
- Split Training & Validation Set
- Fill/Remove Missing Values
- Extract Inputs and Outputs
  
**Feature Engineering**
- Extract Parts of Date
- Add Distance Between Pickup and Drop
- Add Distance From Popular Landmarks
- Remove Outliers and Invalid Data
  
**Train & Evaluate Different Models**
- Split Inputs & Targets
- Random Forest
- Gradient Boosting
  
# Results
From the EDA
1. The busiest day of the week is Friday
![image](https://github.com/user-attachments/assets/e12074b9-a0d0-4550-abd7-19a3cece488c)

2. The busiest time of the day is within 19:00

 ![image](https://github.com/user-attachments/assets/5b4832c4-b361-4709-800c-4b7f619d5a73)

3. The month of August has the highest average fare of $11.74

![image](https://github.com/user-attachments/assets/2eedc176-3a4e-485e-8ff3-f74f9dddbdce)

4. The average ride distance is 20.19 km

5. one percent of the dataset was trained with using different models. The results are as shown below
   |Model|RMSE|
   |-----|----|
   |RandomForestRegressor|3.623353201468282|
   |XGBRegressor|3.1693218|
the gradient boosting model gave a lower RMSE and therefore a better model for prediction


