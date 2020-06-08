#  Predicting Taxi Fares with Deep Feedforward Networks

Technology stack:


The dataset for this project is hosted by Kaggle.<br>
https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data<br>
It has features like pickup_datetime, pickup_longitude, pickup_latitude, dropoff_longitude, dropoff_latitude and passenger_count.<br>
<br>
![Dataset](/images/Dataset_head.PNG)
<br>
<br>
<br>
### Notebooks:<br>
<br>
1. visualization.ipynb:<br>
Plots pick up locations in New York.<br>
<br>
![Pick_up_locations](/images/Plot_lat_long.png)
<br>
<br>
<br>
2. utils.ipynb:<br>
Contains preprocessing which removes outliers, missing values, replaced certain outliers with mode and feature engineering.<br>
<br>
<br>
3. main.ipynb:<br>
Used a Keras model with TensorFlow backend with 5 hidden layers: 1st layer - 128 hidden units with relu activation, 2nd layer - 64 hidden units with relu activation, 3rd layer - 32 hidden units with relu activation, 4th layer - 8 hidden units with relu activation and 5th layer - 1 output unit.<br>
Used Mean squred error as the loss function and adam optimizer with 5 epoches of training.


### Evaluation metrics:<br>
Root Mean Squared Error:<br>
Train RMSE: 3.34<br>
Test RMSE: 3.29<br>
<br>
Prediction on test data:<br>
![Predictions](/images/Prediction.PNG)
