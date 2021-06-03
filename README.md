# Python API Project 

## Background

### WeatherPy: Utilizes weather data from OpenWeather API to find a correlation between various variables. 

### VacationPy: Uses Google Maps API to find ideal vacation hotels based on set weather.

## Part I - WeatherPy

[WeatherPy Script](/WeatherPy/WeatherPy.ipynb)

### Scatter Plots

* Temperature (F) vs. Latitude
<img src="/WeatherPy/City Latitude vs Max Temp.png" alt="My cool logo"/>
* Humidity (%) vs. Latitude
<img src="/WeatherPy/City Latitude vs Humidity.png" alt="My cool logo"/>

* Cloudiness (%) vs. Latitude
<img src="/WeatherPy/City Latitude vs Cloudiness.png" alt="My cool logo"/>

* Wind Speed (mph) vs. Latitude
<img src="/WeatherPy/City Latitude vs Windspeed.png" alt="My cool logo"/>

### Linear Regressions

* Northern Hemisphere - Temperature (F) vs. Latitude
<img src="/WeatherPy/NorthHemisphere_Regression_MaxTemp.png" alt="My cool logo"/>

* Southern Hemisphere - Temperature (F) vs. Latitude
<img src="/WeatherPy/SouthHemisphere_Regression_MaxTemp.png" alt="My cool logo"/>

* Northern Hemisphere - Humidity (%) vs. Latitude
<img src="/WeatherPy/NorthHemisphere_Regression_Humidity.png" alt="My cool logo"/>

* Southern Hemisphere - Humidity (%) vs. Latitude
<img src="/WeatherPy/SouthHemisphere_Regression_Humidity.png" alt="My cool logo"/>

* Northern Hemisphere - Cloudiness (%) vs. Latitude
<img src="/WeatherPy/NorthHemisphere_Regression_Cloudiness.png" alt="My cool logo"/>

* Southern Hemisphere - Cloudiness (%) vs. Latitude
<img src="/WeatherPy/SouthHemisphere_Regression_Cloudiness.png" alt="My cool logo"/>
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
<img src="/WeatherPy/NorthHemisphere_Regression_Windspeed.png" alt="My cool logo"/>
* Southern Hemisphere - Wind Speed (mph) vs. Latitude
<img src="/WeatherPy/SouthHemisphere_Regression_Windspeed.png" alt="My cool logo"/>

## Observations: 

1) According to the "Southern Hemisphere - City Latitude vs. Windspeed" linear regression, there appears to be a negative correlation between latitude and windspeed in the Souther Hemisphere cities.

2) There is a negative correlation between City Latitude and Max Temperature for cities in the Northern Hemisphere.

3) There appears to be a positive correlation between City Latitude and Cloudiness in the Northern Hemisphere.


### Part II - VacationPy

Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

* **Note:** Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out [Google Maps Platform Billing](https://developers.google.com/maps/billing/gmp-billing#monitor-and-restrict-consumption) and [Manage your cost of use](https://developers.google.com/maps/documentation/javascript/usage-and-billing#set-caps) for more information.

* **Note:** if you having trouble displaying the maps, try running `jupyter nbextension enable --py gmaps` in your environment and retry.

To complete this part of the assignment,you will need to do the following:

* Create a heat map that displays the humidity for every city from Part I.

  ![heatmap](Images/heatmap.png)

* Narrow down the DataFrame to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

  * **Note:** Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

  ![hotel map](Images/hotel_map.png)
