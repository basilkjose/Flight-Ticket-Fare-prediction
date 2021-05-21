



![maxresdefault (1)](https://user-images.githubusercontent.com/37875797/119112462-ba874580-ba41-11eb-9e5a-8c2ef0085233.jpg)
## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Data ](#data)
  * [Feature Engineering](#feature-engineering)
  * [Modeling](#modeling)
  * [Technical Aspect](#technical-aspect)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Directory Tree](#directory-tree)
  * [To Do](#to-do)
  * [Technologies Used](#technologies-used)

## Demo
Web App Link - https://flightfarepredictors.herokuapp.com/predict

![Screenshot (196)](https://user-images.githubusercontent.com/37875797/119140894-4dd07300-ba62-11eb-84f7-8d773bb553dc.png)



## Overview
Flight ticket prices can be something hard to guess, today we might see a price, check out the price of the same flight tomorrow, it will be a different story. We might have often heard travellers saying that flight ticket prices are so unpredictable. Huh! Here we take on the challenge! As data scientists, we are gonna prove that given the right data anything can be predicted.

## Data
Dataset-https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh

This Project is used to predict the flight prices. We will use Flight Price Dataset provided by Kaggle Flight Price. This dataset consists of 10683 records with 13 columns that explain about the flight in India by some Indian and foreign Airlines in 2019.

 -- FEATURES --
 
* Airline: The name of the airline.
* Date_of_Journey: The date of the journey
* Source: The source from which the service begins.
* Destination: The destination where the service ends.
* Route: The route taken by the flight to reach the destination.
* Dep_Time: The time when the journey starts from the source.
* Arrival_Time: Time of arrival at the destination.
* Duration: Total duration of the flight.
* Total_Stops: Total stops between the source and destination.
* Additional_Info: Additional information about the flight
* Price: The price of the ticket

## Feature Engineering
*  Made features for Day and Month out of Date of Journey
*  Made features for departure hour and departure minute out of departure time.
*  Made features for arrival hour and arrival minute out of arrival time.
*  Calculated the total flight duration

## Modeling
It is a machine learning regression preoblem.

Algorithms used
* Extra Trees Regressor

Metric - Since the target variable is a continuous variable, regression evaluation metric RMSE (Root Mean Squared Error) and R2 Score (Coefficient of Determination) have been use

* Test R2 Score = 0.812
* Test RMSE Score = 2015.6

## Technical Aspect
This project is divided into two part:

1) Training imdb dataset using machine learning models
2) Deployement of model

* For training purposes, we use sklrean library.
* For deployment, we use Flask and Heroku.

## Deployement on Heroku
![Screenshot (197)](https://user-images.githubusercontent.com/37875797/119140674-14980300-ba62-11eb-942d-d5dca1b1d4c5.png)

For more information read this [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

## Directory Tree 
```
├── static 
│   ├── css
├── template
│   ├── home.html
├── Procfile
├── README.md
├── app.py
├── flight_price.ipynb
├── flight_rf.pkl
├── requirements.txt
```
## To Do
* Use multiple Algorithms
* Optimize Flask app.py
* Front-End 

## Technologies Used
![](https://forthebadge.com/images/badges/made-with-python.svg)

* Flask
* Heroku
* Sklearn
* Google colab
