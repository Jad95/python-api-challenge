# python-api-challenge

# Weather_Analysis

## Main Objective
1-Perform tasks using new Python libraries and modules.
2-Pandas, gmaps, requests, numpy, random, matplotlib, timeit, scipy, citipy, datetime, time
3-Retrieve and use data from an API "get" request to a server.
4-Retrieve and store values from a JSON array.
5-Use try and except blocks to resolve errors.
6-Write Python functions.
7-Create scatter plots using the Matplotlib library, and apply styles and features to a plot.
8-Perform linear regression, and add regression lines to scatter plots.
9-Create heatmaps, and add markers using the Google Maps API.

# Overview
This challenge includes two parts:

## Part 1 - WeatherPy
Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you’ll be utilizing a simple Python library, Citipy, and the OpenWeatherMap API.

The first requirement is to create a series of scatter plots to showcase the relationships between location and temperature, humidity, wind speed, and cloudiness.

The second requirement is to run linear regression on each relationship for the northern and southern hemispheres.

Steps to follow:
Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it’s being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Part 2 - VacationPy
Work with weather data created in Part I to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.
Narrow down the dataframe to find your ideal weather condition. For example:
A max temperature lower than 80 degrees but higher than 70.
Wind speed less than 10 mph.
Zero cloudiness.
Drop any rows that don’t contain all three conditions. You want to be sure the weather is ideal.
Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

# Process
Retrieve the Weather Data

An API was established with OpenWeatherMap and a DataFrame was created to get the initial list of potential cities.
![Alt text](image-1.png)

# Statistical Analysis
Global city data was plotted, and linear regression was used to find the relationship between the following variables:

Latitude and Maximum Temperature
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/145f0f9b-1652-4044-8026-c418f39559ce)
Latitude and Humidity
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/36f31809-2487-4680-af7f-03c9d3246885)
Latitude and Cloudiness
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/eb882828-ea92-4dc2-aa52-3db1233a0325)
Latitude and Wind Speed
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/8c47aefe-8f0c-4976-a0a1-5b3f4103e3b1)

# Linear Regression on the Northern and Southern Hemispheres
Linear regression was performed for the Northern and Southern Hemispheres, on all four weather parameters: maximum temperature, humidity, cloudiness, and wind speed.

Maximum Temperature
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/509c2559-fa31-4db8-b1ca-893568b4cb6f)
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/f78dc0f5-b181-4e34-9bdf-2d9029282cfc)

Percent Humidity
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/2b5e8762-7905-4718-bd7a-625264684b1f)
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/044233f4-a39e-4d1b-aea9-315eed6afae9)

Percent Cloudiness
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/56666509-f6ff-48b8-9b4f-58e7d519682a)
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/3a2c70f5-f9bf-40af-a282-ccf8a439ee3d)

Wind Speed
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/e7c3ee6d-dc4e-4d30-9788-433c299c7ba8)
![image](https://github.com/Jad95/python-api-challenge/assets/130928755/adf27856-0698-4e74-a5f7-ea769fde8c99)
