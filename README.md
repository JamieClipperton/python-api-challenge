# python-api-challenge - Whats the Weather Like?

## Part I - WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude

![image](https://user-images.githubusercontent.com/101610081/181096601-c014ecba-07d0-4946-9751-8a3ae99a026f.png)


* Humidity (%) vs. Latitude

![image](https://user-images.githubusercontent.com/101610081/181096670-47309567-611c-4e96-93a5-97a4e2cf612a.png)

* Cloudiness (%) vs. Latitude

![image](https://user-images.githubusercontent.com/101610081/181096728-e4bfb2b0-0f6a-4671-a02d-a35dad1241c6.png)

* Wind Speed (mph) vs. Latitude

![image](https://user-images.githubusercontent.com/101610081/181096780-12e1e62d-1abe-4dbb-85c8-cb23005d0ba0.png)


The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![image](https://user-images.githubusercontent.com/101610081/181097107-805854ad-e64a-4375-bb75-b072c5d1e457.png)
![image](https://user-images.githubusercontent.com/101610081/181097143-b741032e-7ab7-4bcb-90e7-9e9adbf7ef70.png)
![image](https://user-images.githubusercontent.com/101610081/181097174-84c15ca4-fc58-464b-b056-4b0191210a50.png)
![image](https://user-images.githubusercontent.com/101610081/181097298-cfdcea50-8bd5-4237-ac4e-2a10b8a39c6e.png)
![image](https://user-images.githubusercontent.com/101610081/181097326-c2a36420-4b92-4da5-80fd-e85560ac3816.png)
![image](https://user-images.githubusercontent.com/101610081/181097363-3cb326dd-f994-487a-b29b-0b5f5f5573cb.png)
![image](https://user-images.githubusercontent.com/101610081/181097421-48942fe1-0f53-4e6d-89dd-4eb7ca56e7ee.png)
![image](https://user-images.githubusercontent.com/101610081/181097459-64336a35-9152-4789-bf70-3d583701f72e.png)

## Observations

* Southern Hemisphere stays warmer then the Northern Hemisphere based on minimum Tempatures.
* There is no signfigant correlation between humidity and latitude.
* Wind Speeds do not have a signifigant change between north and south hemispheres. 


## Part II - VacationPy

* Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

* Create a heat map that displays the humidity for every city from Part I.

![image](https://user-images.githubusercontent.com/101610081/181098571-84931e87-338f-4acf-83c9-e8b994d954d1.png)

* Narrow down the DataFrame to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

  * **Note:** Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

![image](https://user-images.githubusercontent.com/101610081/181098784-3ecba04c-fed1-47e3-a37d-f02eed56f009.png)




