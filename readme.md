<!-- project Title: -->
 Vehicle Price Prediction using Machine Learning

<!-- Objective: -->
The goal of this project to predict the resale the price of a used vehicle according to its own features.By analyzing the details like the car's make,model,year,mileage,and fuel type,the model predict the selling price.This kind of prediction is useful for both sellers and buyers.


<!-- Dataset Infromation: -->
this data set is provided by intership company.it contains 1000 records of vehicles.the target column is "price",which we want to prict.
features included:make, model, year, fuel, transmission, mileage, body, doors, exterior_color, interior_color

<!-- Steps followed by me: -->
1. loaded a dataset using pandas and checked its shape ,columns types and missing values.
2. handle the missing values:
  -for the categorical columns(fuel,transmission,doors etc.),i used mode to fill most frequent value.
  -for numerical columns like mileage and cylinders,i used the median.
3. drop the engine columns it contains messy data that is hard to clean and use
4. converted columns cylinders from text to numbers.
5. i know that ml only understand the numbers, i used label enocding to convert text categories into numerical values using LabelEncoder from sklearn
6. I used train_test_split from sklearn to divide the dataset into training and testing sets:
-80% of the data for training the model
-20% of the data for testing it
7. I used the Linear Regression model from `scikit-learn` to predict the vehicle prices. 

<!-- what i learned: -->
-i learned how to loead , clean, and understand a real world data set.
-understand the difference between mode and median fro missing data
-i practice converting text based data into numeric
-i learn the importance of checking the type of data 
-also i learned not all the columns are useful and drop them is simplify the model
-learn to use labelencoder to convert categorical data into numbers 
-i learned how to split the data using train_test_split from sklearn, which helps to divide the data set into traing and testing parts.
- How to evaluate model performance using MSE and R² score
- That not all features are useful — some may need to be dropped
-This model helps to find a straight-line relationship between the vehicle features and its price.

<!-- result -->
after evaluating the model ,i got:
Mean squared error (MSE)-220,844,759
R-squared Score(R**2):0.27


<!-- Author -->
Apurva Guleria
ML intern @Unified Mentor



