# Amaliy_Loyhalar

Airfare Price Prediction
This project is focused on predicting airfare prices using machine learning techniques. The model is trained using historical flight data and applies a RandomForestRegressor to predict future prices. The pipeline is built using numerical and categorical preprocessing techniques, and the final predictions are stored in a CSV file for evaluation or further use.

Project Overview
This project uses:

Pandas for data manipulation.
Scikit-learn for preprocessing and machine learning model creation.
A RandomForestRegressor model for price prediction.
A cross-validation technique to evaluate the model's accuracy based on R² scoring.
Dataset
The following datasets are required to run the project:

train_data.csv: The training dataset that contains flight information and corresponding airfare prices.
test_data.csv: The test dataset that contains flight information for which the prices need to be predicted.
sample_solution.csv: A sample solution file to store the predicted prices.
Features
Numerical Features:

duration: Flight duration.
days_left: Days left until departure.
Categorical Features:

airline: Name of the airline.
flight: Flight number.
source_city: City of departure.
departure_time: Departure time of the flight.
stops: Number of stops.
arrival_time: Arrival time of the flight.
destination_city: City of arrival.
class: Travel class (e.g., Economy, Business).
Steps
Data Preprocessing:

The numerical features are scaled using StandardScaler.
The categorical features are one-hot encoded using OneHotEncoder.
A full pipeline (ColumnTransformer) is created to handle both types of features.
Model Training:

The RandomForestRegressor model is trained on the preprocessed training dataset.
Model Evaluation:

The model's accuracy is evaluated using cross-validation with the R² score as the metric.
Prediction:

The model predicts the prices for the test dataset, and the results are saved to the air_prediction.csv file.
Code Execution
Install the required libraries:

bash
Copy code
pip install pandas scikit-learn numpy
Make sure your train_data.csv, test_data.csv, and sample_solution.csv files are in the correct directory.

Run the Python script:

bash
Copy code
python airfare_price_prediction.py
The predicted airfare prices will be saved in air_prediction.csv.

Output
The model’s R² accuracy score will be printed in the console.
The predicted prices for the test dataset will be saved in the air_prediction.csv file.
Example
Here's how to run the script and interpret the output:

bash
Copy code
Modelning R^2 aniqligi: 85.76%
Natijalar 'air_prediction.csv' faylga saqlandi.
