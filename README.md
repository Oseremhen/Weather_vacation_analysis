# What is the weather like as we approach the equator?

Background: Data's true power is its ability to definitively answer questions. So, let's take Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

<img width="301" alt="Screenshot 2023-01-21 at 6 31 52 AM" src="https://user-images.githubusercontent.com/106120403/213865106-a8e71eae-a992-4a1e-be86-c6163ba00716.png">


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

![Fig1](https://user-images.githubusercontent.com/106120403/213865230-d57c9e0a-869f-4a56-94db-1cd4c9249e03.png)

Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude

![Fig2](https://user-images.githubusercontent.com/106120403/213865223-0a0c12c8-32b4-430b-a270-a8ee24e84f4a.png)

Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude

![Fig3](https://user-images.githubusercontent.com/106120403/213865203-22799339-c676-4863-afe2-48c0ea08e752.png)

Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

![Fig4](https://user-images.githubusercontent.com/106120403/213865189-b7ce5055-c1ef-4ff9-b1aa-a6c83ce9e652.png)

Part 2: VacationPy.ipynb:

In this deliverable, I used used Jupyter notebooks, the geoViews Python library, and the Geoapify API to plan future vacations. I employed my Python skills to create map visualizations using Geoapify API and geoViews Python library. I create a map that displays a point for every city in the city_data_df DataFrame made the humidity in each city the size of the points, narrowed down the city_data_df DataFrame to find your ideal weather condition (i.e. zero cloudiness and a max temperature lower than 28 degrees but higher than 20).

<img width="1032" alt="Screenshot 2023-01-21 at 6 38 49 AM" src="https://user-images.githubusercontent.com/106120403/213865273-a28195ed-1a26-417c-b11f-efcf996c41e0.png">

I created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity and for each city, I used the Geoapify API to find the first hotel located within 10,000 meters of my coordinates, then I added the hotel name and the country as additional information in the hover message for each city on the map.

<img width="1032" alt="Screenshot 2023-01-21 at 6 40 03 AM" src="https://user-images.githubusercontent.com/106120403/213865286-8aa4900c-cd2e-4088-a23e-a55cf702159c.png">
