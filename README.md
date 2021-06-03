# Python API Project 

## Background

### WeatherPy: Utilizes weather data from OpenWeather API to find a correlation between various variables. 

### VacationPy: Utilizes Google Maps API to find ideal vacation hotels based on set weather.

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

[VacationPy Script](/VacationPy/VacationPy.ipynb)

## Heatmap 

<img src="/VacationPy/Heat Map.png" alt="My cool logo"/>
 

* Narrowing down the DataFrame ideal weather conditions:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.


* Plotting the top hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country** based on ideal weather conditions.
<img src="/VacationPy/Hotel Point Map.png" alt="My cool logo"/>

