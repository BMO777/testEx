# python-api-challenge

Uses OpenWeatherApi and Geoapify api. The Former to take city name data generated by citipy module to request weather data collected depending on day, then geoapify is used  to narrow down criterion to help select where would be ideal weather and thereby an ideal place to vacation or live


The data extracted from the Openweather api is saved to a csv file, then bound in a dataframe including, Maximum temperature, Latitude&Longitude, City,	Humidity, Cloudiness,	Wind Speed,	&Country.

In the Weatherpy Notebook, Latitude is compared to Maximum temperature, Humidity, Cloudiness,	and Wind Speed, then charted to a scatter plot to visualize those comparisons. 

Next, the latitude is sepatated into two data frames, one for the northern hemispere and the other for the southern, and a linear regression line is formulated to show whether any relationship between those aforementioned variables and Latitude is present within the two hemispheres ranging from closer to the equator to farther away.

In the Vacationpy notebook, the csv saved from the OpenaWeatherApi data in WeatherPy is used to narrow down best potential vacation locations and display them within  points of a map using the hvplot module in pandas. I used the criteria that the location must be within the range of latitudes between -50 to 40, that the Maximum temperature must be greater than or equal to 25°C(77°F), and that the cloudiness must be less than or equal to around 25%. 

Then using the Geoapify api, locations within 10000 meters of the longitudes and latitudes for each city derived from the Citipy module are searched for accomodations. I did not narrow down this to search for hotels only, but all accomodations, such as short term house rental services and hostels. This is also displayed in points within a map using hvplot module at the end of the notebook.


