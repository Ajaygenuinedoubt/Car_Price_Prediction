# Car_Price_Prediction
Car Price Prediction App


This project is an interactive Car Price Prediction App built using Streamlit and a machine learning model (Ridge Regression). The app allows users to input various car features and predicts the price of a car based on the given inputs.

## Features

Interactive Dashboard: Users can input car features using an intuitive sidebar and get instant predictions.

Ridge Regression Model: A Ridge regression model is used to predict car prices.

Efficient Caching: The dataset and model are cached using Streamlit's @st.cache_data and @st.cache_resource for faster performance.

## Technologies Used

Streamlit: For building the user interface and dashboard.

Scikit-learn: For data preprocessing and machine learning.

Pandas: For data manipulation and loading.

Python: The core programming language.

Installation Instructions
Follow these steps to set up the project on your local machine:

## Step 1: Clone the Repository

git clone https://github.com/yourusername/car-price-prediction-app.git

cd car-price-prediction-app

## Step 2: Install the Required Packages
Install the necessary libraries by running:

pip install -r requirements.txt
You can manually install the main dependencies if requirements.txt is not provided:


pip install streamlit pandas scikit-learn matplotlib seaborn


## Step 3: Running the Application
Run the Streamlit application by executing the following command:


streamlit run car_price_prediction.py
This will launch the app in your default web browser.

## Dataset

The car price dataset used in this project can be found in the car.csv file. The dataset contains features such as:

symboling
fueltype
aspiration
carbody
drivewheel
enginelocation
And more...

Ensure the car.csv file is in the same directory as the project script or update the path to load the dataset properly.

## Project Overview
Data Preprocessing:

The dataset is cleaned by handling missing values and dropping unnecessary columns like car_ID and CarName.

Categorical columns are one-hot encoded, and numerical columns are scaled for better model performance.

## Machine Learning Model:

A Ridge Regression model is used for predicting car prices. The model pipeline includes preprocessing steps and is trained using the dataset.

The Mean Squared Error (MSE) is calculated to evaluate the model's performance.

## Interactive Dashboard:

The app provides a sidebar where users can input various car features such as fueltype, cylindernumber, horsepower, and more.

After inputting the car features, users can press the "Predict" button to get the car price prediction instantly.

## Caching Mechanism:

The dataset and trained model are cached using Streamlit’s @st.cache_data and @st.cache_resource to reduce reloading time and improve efficiency.
User Interface

## The app consists of:

Main Dashboard: Displays dataset information and model performance metrics (MSE).

Sidebar: Allows users to input car features like engine type, fuel type, horsepower, etc.

Predict Button: Once the user inputs the data, they can predict the car price by clicking the button.

## How It Works
The user enters car specifications via the sidebar.

The model predicts the car price based on the input features.

The predicted price is shown in real-time on the sidebar.

## Example Features for Prediction

Symboling: A slider ranging from -3 to 3.

Fuel Type: Options like gas or diesel.

Aspiration: Options like standard or turbo.

Cylinders: The number of cylinders in the engine (e.g., four, six).

Horsepower: A slider for specifying horsepower.

And many more...

## Model Performance

The Ridge Regression model was evaluated using Mean Squared Error (MSE). You can view the MSE value on the main dashboard when the app is running.

## Future Improvements

Add more advanced machine learning models for better accuracy.

Enhance the UI design for improved user experience.

Enable users to upload their own datasets for custom predictions.
