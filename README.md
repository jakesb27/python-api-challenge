# Python API Challenge

#### UCI Data Analytics Bootcamp | Module 6 Challenge

<br />

## Summary

This is a two part challenge consisting of [WeatherPy](#weatherpy) and [VacationPy](#vacationpy). Both scripts use free public API's to obain necessary information. [WeatherPy](#weatherpy) uses the <a href="https://openweathermap.org/api">OpenWeather API</a> to obtain the weather information of a random list of cities. The datapoints are then analyzed for any trends or correlations. [VacationPy](#vacationpy) uses the <a href="https://www.geoapify.com/get-started-with-maps-api">Geoapify</a> API to gather hotels closest to some of the cities in the list of cities gathered in the previous script. These are then mapped to provide a visual representation of places to vacation.

<br />

## Table of Contents
#### [Part I - WeatherPy](#weatherpy)

* [Scatter Plotting](#scatter-plotting)
  * [Latitude vs. Temperature](#latitude-vs-temperature)
  * [Latitude Vs. Humidity](#latitude-vs-humidity)
  * [Latitude Vs. Cloudiness](#latitude-vs-cloudiness)
  * [Latitude vs. Wind Speed](#latitude-vs-wind-speed)
* [Linear Regression Plotting](#linear-regression-plotting)
  * [Temperature vs. Latitude](#temperature-vs-latitude)
    * Northern Hemisphere
    * Southern Hemisphere
  * [Humidity vs. Latitude](#humidity-vs-latitude)
    * Northern Hemisphere
    * Southern Hemisphere
  * [Cloudiness vs. Latitude](#cloudiness-vs-latitude)
    * Northern Hemisphere
    * Southern Hemisphere
  * [Wind Speed vs. Latitude](#wind-speed-vs-latitude)
     * Northern Hemisphere
     * Southern Hemisphere

#### [Part II - VacationPy](#vacationpy)

 * [Geo Map Plotting](#geo-map-plotting)
   * [All Cities Without Hotel](#all-cities-without-hotel)
   * [My Selected Cities With Hotel](#my-selected-cities-with-hotel)

<br />

## WeatherPy


In WeatherPy a list of 500+ random cities was generated using NumPy's random function to create random sets of longitue and latitude coordinates. These coordinates were then fed into the citypy module to obtain the name of the nearest city. The cities were saved in a csv to be accessed later. Using the complete dataset, various scatter plots were generated to visualize different datapoints against the city's latitude.

<br />

<table class="dataframe" border="1">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>City</th>
      <th>Lat</th>
      <th>Lng</th>
      <th>Max Temp</th>
      <th>Humidity</th>
      <th>Cloudiness</th>
      <th>Wind Speed</th>
      <th>Country</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>rikitea</td>
      <td>-23.1203</td>
      <td>-134.9692</td>
      <td>78.48</td>
      <td>76</td>
      <td>8</td>
      <td>12.71</td>
      <td>PF</td>
      <td>1675563787</td>
    </tr>
    <tr>
      <th>1</th>
      <td>hobart</td>
      <td>-42.8794</td>
      <td>147.3294</td>
      <td>76.05</td>
      <td>45</td>
      <td>20</td>
      <td>6.91</td>
      <td>AU</td>
      <td>1675563619</td>
    </tr>
    <tr>
      <th>2</th>
      <td>ushuaia</td>
      <td>-54.8000</td>
      <td>-68.3000</td>
      <td>51.46</td>
      <td>76</td>
      <td>40</td>
      <td>6.91</td>
      <td>AR</td>
      <td>1675563750</td>
    </tr>
    <tr>
      <th>3</th>
      <td>arraial do cabo</td>
      <td>-22.9661</td>
      <td>-42.0278</td>
      <td>76.33</td>
      <td>91</td>
      <td>17</td>
      <td>7.47</td>
      <td>BR</td>
      <td>1675563645</td>
    </tr>
    <tr>
      <th>4</th>
      <td>nerang</td>
      <td>-27.9833</td>
      <td>153.3333</td>
      <td>91.38</td>
      <td>66</td>
      <td>65</td>
      <td>7.00</td>
      <td>AU</td>
      <td>1675563789</td>
    </tr>
  </tbody>
</table>

[Back To Top](#python-api-challenge)

<br />

## Scatter Plotting

<br />

### Latitude Vs. Temperature

![Fig1](https://user-images.githubusercontent.com/82631980/216805291-23adccfd-3f31-4cf0-87be-5ca5d38c2e28.png)

[Back To Top](#python-api-challenge)
<br />
<br />

### Latitude Vs. Humidity

![Fig2](https://user-images.githubusercontent.com/82631980/216805298-46c4738b-b1d5-4f54-9059-1ac46dcaf6fa.png)

[Back To Top](#python-api-challenge)
<br />
<br />

### Latitude Vs. Cloudiness

![Fig3](https://user-images.githubusercontent.com/82631980/216805300-816d9d40-c9fe-4102-80e1-c82c2a370f1f.png)

[Back To Top](#python-api-challenge)
<br />
<br />

### Latitude vs. Wind Speed

![Fig4](https://user-images.githubusercontent.com/82631980/216805302-ecd47856-b231-429b-ba47-0eadf3d91399.png)

[Back To Top](#python-api-challenge)
<br />
<br />

## Linear Regression Plotting

<br />
<u>

## Temperature Vs. Latitude
</u>

For the Northern Hemisphere, there is a high negative correlation coefficient that indicates that the further North one travels, the colder the max temperate is this time of the year. However, for the Southern Hemisphere, there is a low positive correlation coefficient that suggests there is no strong direct relationship between the distance traveled south and the max temperature during this time of the year.

<br />

### Northern Hemisphere
![tln](https://user-images.githubusercontent.com/82631980/216807134-0f901db1-b3a1-4764-af83-7dfc7f5de35c.png)

### Southern Hemisphere
![tls](https://user-images.githubusercontent.com/82631980/216807143-8f4a99ae-7a0d-4ef8-ae05-a6e6f6537716.png)

[Back To Top](#python-api-challenge)

<br />
<br />
<u>

## Humidity Vs. Latitude

</u>

For the Northern and Southern Hemispheres, there is a mid to low positive correlation coefficient between the humidity and the latitude. Interesting enough both graphs are positive with the Southern Hemisphere having a y-intercept at 84% humidity and the Northern having a y-intercept at 58% humidity, with the y-intercept representing the equator. The increase in humidity from the equator to the distance traveled North in the Northern Hemisphere is greater than the increase in humidity from the distance traveled South to the equator.

### Northern Hemisphere
![hln](https://user-images.githubusercontent.com/82631980/216807169-43b5da15-057c-4e7e-be40-263d533e31dc.png)

### Southern Hemisphere
![hls](https://user-images.githubusercontent.com/82631980/216807174-084ea7f4-4b64-45d0-8669-82a4866684f1.png)

[Back To Top](#python-api-challenge)

<br />
<br />
<u>

## Cloudiness Vs. Latitude

</u>

There is little to no relationship between the altitude and the cloudiness. The plotted points are sporadic and not uniform with the y-axis ranging from 0 to 100 with just an increase of 1, if any increase at all, on the x-axis.

### Northern Hemisphere
![cln](https://user-images.githubusercontent.com/82631980/216807184-59180be8-ab2e-4e4e-bfca-cf535170d901.png)

### Southern Hemisphere
![cls](https://user-images.githubusercontent.com/82631980/216807190-9b5598bf-87c3-4cfd-a246-e8282f585c46.png)

[Back To Top](#python-api-challenge)

<br />
<br />
<u>

## Wind Speed Vs. Latitude

</u>

There is little to no relationship between the altitude and the wind speeds. The wind speeds do not have a wide range and are not uniform.

### Northern Hemisphere
![wln](https://user-images.githubusercontent.com/82631980/216807196-54a1bce2-6f29-4099-a8c6-70f792339639.png)

### Southern Hemisphere
![wls](https://user-images.githubusercontent.com/82631980/216807200-28f225e4-bc46-4e50-8477-44696261698e.png)

[Back To Top](#python-api-challenge)

<br />
<br />

## VacationPy

VacationPy takes the list of cities in [WeatherPy](#weatherpy) and maps them using hvplot with the dot size being the humidity percentage. This list of cities is then filtered down based on my own personal preferred weather conditions for a sweet vacation. We then utilize Geoapify's API to obtain the nearest hotel within 10,000 meters and save it to our dataframe. The list is then replotted on a map to inlcude the weather and hotel information when the mouse if hovered over the selection.

<br />
<br />

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>City_ID</th>
      <th>City</th>
      <th>Lat</th>
      <th>Lng</th>
      <th>Max Temp</th>
      <th>Humidity</th>
      <th>Cloudiness</th>
      <th>Wind Speed</th>
      <th>Country</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>rikitea</td>
      <td>-23.1203</td>
      <td>-134.9692</td>
      <td>78.48</td>
      <td>76</td>
      <td>8</td>
      <td>12.71</td>
      <td>PF</td>
      <td>1675563787</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>hobart</td>
      <td>-42.8794</td>
      <td>147.3294</td>
      <td>76.05</td>
      <td>45</td>
      <td>20</td>
      <td>6.91</td>
      <td>AU</td>
      <td>1675563619</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>ushuaia</td>
      <td>-54.8000</td>
      <td>-68.3000</td>
      <td>51.46</td>
      <td>76</td>
      <td>40</td>
      <td>6.91</td>
      <td>AR</td>
      <td>1675563750</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>arraial do cabo</td>
      <td>-22.9661</td>
      <td>-42.0278</td>
      <td>76.33</td>
      <td>91</td>
      <td>17</td>
      <td>7.47</td>
      <td>BR</td>
      <td>1675563645</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>nerang</td>
      <td>-27.9833</td>
      <td>153.3333</td>
      <td>91.38</td>
      <td>66</td>
      <td>65</td>
      <td>7.00</td>
      <td>AU</td>
      <td>1675563789</td>
    </tr>
  </tbody>
</table>

[Back To Top](#python-api-challenge)

<br />

## Geo Map Plotting

<br />

### All Cities Without Hotel

![all_cities](https://user-images.githubusercontent.com/82631980/216847272-a333df23-3002-49b4-b9c7-aadfaf0a7283.png)

[Back To Top](#python-api-challenge)

<br />
<br />

### My Selected Cities With Hotel

![my_cities](https://user-images.githubusercontent.com/82631980/216847290-20fa0ca8-54b8-414a-8553-2a33ec874b3d.png)

[Back To Top](#python-api-challenge)

<br />
<br />

## License

[MIT](https://choosealicense.com/licenses/mit/)

<br />
<br />

[Back To Top](#python-api-challenge)
