# Pandas-Api-Challange

Background:

Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"
Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

Part 1: WeatherPy.ipynb:

In this deliverable, I used Python script to visualize the weather of over 500 cities of varying distances from the equator. I used the citipy Python library Links, the OpenWeatherMap API Links to create a representative model of weather across cities.
I used the OpenWeatherMap API to retrieve weather data from the cities list generated and created a series of scatter plots to showcase the following relationships:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

I also separated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude) and created a series of scatter plots (including the linear regression line, the model's formula, and the r values)

The following plots were included with an explanation of what the linear regression is modeling:

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

Part 2: VacationPy.ipynb:

In this deliverable, I used used Jupyter notebooks, the geoViews Python library, and the Geoapify API to plan future vacations. I employed my Python skills to create map visualizations using Geoapify API and geoViews Python library. I create a map that displays a point for every city in the city_data_df DataFrame made the humidity in each city the size of the points, narrowed down the city_data_df DataFrame to find your ideal weather condition (i.e. zero cloudiness and a max temperature lower than 28 degrees but higher than 20).

I created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity and for each city, I used the Geoapify API to find the first hotel located within 10,000 meters of my coordinates, then I added the hotel name and the country as additional information in the hover message for each city on the map.

