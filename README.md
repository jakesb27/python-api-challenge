# Python API Challenge

UCI Data Analytics Bootcamp | Module 6 Challenge

## Table of Contents
* Part I - WeatherPy
  * [Scatter Plotting](##Scatter-Plotting)
    - [Latitude vs. Temperature](###Latitude-Vs.-Temperature)
  
## Part I - WeatherPy

In WeatherPy a list of 500+ random cities was generated using NumPy's random function to create random sets of longitue and latitude coordinates. These coordinates were then fed into the citypy module to obtain the name of the nearest city. The cities were saved in a csv to be accessed later. Using the complete dataset, various scatter plots were generated to visualize different datapoints against the city's latitude.

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

## Scatter Plotting

### Latitude Vs. Temperature
![Fig1](https://user-images.githubusercontent.com/82631980/216805291-23adccfd-3f31-4cf0-87be-5ca5d38c2e28.png)

### Latitude Vs. Humidity
![Fig2](https://user-images.githubusercontent.com/82631980/216805298-46c4738b-b1d5-4f54-9059-1ac46dcaf6fa.png)

### Latitude Vs. Cloudiness
![Fig3](https://user-images.githubusercontent.com/82631980/216805300-816d9d40-c9fe-4102-80e1-c82c2a370f1f.png)

### Latitude vs. Wind Speed
![Fig4](https://user-images.githubusercontent.com/82631980/216805302-ecd47856-b231-429b-ba47-0eadf3d91399.png)

<br></br>

## License

[MIT](https://choosealicense.com/licenses/mit/)




