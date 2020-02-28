# Temperature Analysis by Latitude

This project is an analysis of how various weather-related phenomena change as a function of changes in latitude. 

This project consists of two main notebook files:

1. WeatherPY_DataRetrieval_and_Population.ipynb
- This file cotains code that generates a random list of latitudes and longitudes.
- It then queries CitiPy to find the nearest city to those coordinates, and creates a list of unique cities found from those coordinates
- Using the unique city list, it makes a series of API calls to Open Weather Map to see:
- - Is each city in OWM
- - If so: grab the temperature data for that city and store that in a new list 
- After generating the list of cities with temp data, the file then creates a dataframe and saves that city and temp data to a csv file
- The file also creates a CSV that stores all of the API Call Responses 

2. WeatherPy_ReadFromCSV_and_GeneratePlots.ipynb
- This file reads in the city data from the previously generated CSV
- Then it creates plots investigating the relationship of the following variables:
- - Latitude vs. Max Temp
- - Latitude vs. Humidity 
- - Latitude vs. Cloudiness
- - Latitude vs. Wind Speed


