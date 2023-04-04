# Flight Price Prediction

<div align="center">
<img src="https://user-images.githubusercontent.com/126209562/229326932-f6844e00-2a3e-4186-ba23-5f1583773af8.jpg" width="700px" />
</div>

# 1. Business Problem
### Introduction
  The objective of the study is to analyse the flight booking dataset obtained from “Ease My Trip” website and to conduct various statistical hypothesis tests in order to get meaningful information from it. The 'Linear Regression' statistical algorithm would be used to train the dataset and predict a continuous target variable.
  
### Research Questions
   The aim of our study is to answer the below research questions:
    
    a) Does price vary with Airlines?
    b) How is the price affected when tickets are bought in just 1 or 2 days before departure?
    c) Does ticket price change based on the departure time and arrival time?
    d) How the price changes with change in Source and Destination?
    e) How does the ticket price vary between Economy and Business class?
    
 # FEATURES
 - The various features of the cleaned dataset are explained below:

    - Airline: The name of the airline company is stored in the airline column. It is a categorical feature having 6 different airlines.
    
    - Flight: Flight stores information regarding the plane's flight code. It is a categorical feature.

    - Source City: City from which the flight takes off. It is a categorical feature having 6 unique cities.

    - Departure Time: This is a derived categorical feature obtained created by grouping time periods into bins. It stores information about the departure time and have 6 unique time labels.

    - Stops: A categorical feature with 3 distinct values that stores the number of stops between the source and destination cities.

    - Arrival Time: This is a derived categorical feature created by grouping time intervals into bins. It has six distinct time labels and keeps information about the arrival time.

    - Destination City: City where the flight will land. It is a categorical feature having 6 unique cities.

    - Class: A categorical feature that contains information on seat class; it has two distinct values: Business and Economy.

    - Duration: A continuous feature that displays the overall amount of time it takes to travel between cities in hours.

    - Days Left: This is a derived characteristic that is calculated by subtracting the trip date by the booking date.

    - Price: Target variable stores information of the ticket price.

# 2. Solution Strategy
  My strategy to solve this challenge was:
  
  Step 01. Data Description: My goal is to use statistics metrics to identify data outside the scope of business.
  
  Step 02. Data Filtering: Filter rows and select columns that do not contain information for modeling or that do not match the scope of the business.
  
  Step 03. Exploratory Data Analisys: Explore the data to find insights and better undestand the impact of variables on model training.
  
  Step 04. Answer the questions: Plot graphs to understand the data and then solve the questions.
  
  Step 05. Data Preparation: Prepare the data so that the Machine Learning models can learn the specific behavior.
  
  Step 06. Feature Selection: Selection of the most significant attributes for training the model.
  
  Step 07. Machine Learning Modeling: Machine Learning model training.

# 3. Answering the questions

<div align="center">
<img src="https://user-images.githubusercontent.com/126209562/229897604-24261882-5050-4563-bdfe-cbc8cc74a364.png" width="600px" />
</div>
**R:** Yes, it does. The AirAsia and Vistaria airlines have the highest price while the others have a very similiar average price. 

# 4. Machine Learning Model Applied
- Tests were made using different algorithms:
    - Linear Regression
    - Decision Tree
    - Random Forest
  
# 5. Machine Learning Model Performance
  The chosen algorithm was Random Forest Regression.
  
| Mean Squared Error  | Root Mean Square Error | R-squared  | 
| ------------- | ------------- | ------------- | 
| 0.0012  | 0.0346  | 0.9654  |
