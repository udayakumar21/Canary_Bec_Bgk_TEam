# Canary_Bec_Bgk_TEam
Team Name:642947-U2K4Y208
Team Members are:
1)Kaveri Angadi
2)Mallikarjun Hiremath
3)Rashmi Hiremath
4)Udayakumar Hiremath
Project Title

Predicting soil moisture levels at a specific location based on
the previous 8 months of soil moisture data along with
temperature, and humidity values at the location.

Description
First we integrated user1_data with user2_data (st column in user1_data is integrated with user2_data.csv file as that column was missing earlier in user2_data.csv)
We implemented our model in google collab. Our model uses Facebook Prophet to predict soil moisture for the next month based on historical data. The script loads a CSV file with historical user soil moisture data, trains a Prophet model on the data, and then makes predictions for the next month.


The predict_soil_moisture.py script is a Python implementation of Facebook Prophet, which is a forecasting tool that is designed to make accurate predictions based on time-series data. This script uses Prophet to predict soil moisture for the next month based on historical data.

The script first loads the historical soil moisture data from a CSV file using the pandas library. The timestamp column in the data is then converted to a datetime object, and the month is extracted from the timestamp. The columns are then renamed to 'ds' (timestamp) and 'y' (soil moisture) to fit the Prophet's input format.

The Prophet model is then trained on the historical data using the fbprophet library. Next, a new DataFrame is created to hold the timestamps for each day in March 2022, and the model is used to make predictions for each day in the DataFrame.

Finally, the predicted soil moisture values for each day in March 2022 are printed to the console.


Dependencies
pandas
fbprophet

Usage
The script will output the predicted soil moisture values for each day in March 2023 to the console.
