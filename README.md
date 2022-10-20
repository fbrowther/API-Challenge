## PythonAPIChallenge

# WeatherPy

Weather of 500+ cities across the world of varying distance from the equator was obtained (randomly) using the OpenWeatherMap API. The data obtained was cleaned, and a panda dataframe was created. Using this dataframe, a series of analysis to determine the relationship of different variables was carried out and this included -

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

Data was then separated based on whether citied were located in the northern (greater than or equal to 0 degrees latitude) or sourthern (less than 0 degrees latitude) hemisphere and a series of linear regression on each relationship

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

Retrieved data was saved as a CSV file along with PNG image for each scatter plot.


# VacationPy

Employing google maps (gmaps), a heatmap that displays the humidity data for every city generated from WeatherPy was created.

WeatherPy DataFrame was narrowed to find an ideal weather condition such as
(i) City temperature between 70 and 80 degrees F.
(ii) Wind speed less than 10 mph.
(iii) Zero cloudiness.

Employing Google Places API, hotels located within 5000 meters of city coordinates was determined and the hotels were plotted on google maps on top of the humidity heatmap


# Important initial requirements:
(1) Create API Keys on (a) OpenWeatherMap (https://openweathermap.org/) and store it as 'weather_api_key'in a config file
(2) Create Google API Key (https://console.developers.google.com/getting-started) and store it as 'g_key' in the same config file.
(3) From the local terminal add the config file (containing API keys) onto the '.gitignore' file so user credentials and API keys are not exposed.
(4) Install citipy in your python environment (https://pypi.python.org/pypi/citipy)
