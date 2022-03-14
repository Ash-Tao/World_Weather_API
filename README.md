# python_api_challenge

### Task 1: WeatherPy 
Visualize the weather of 500+ cities of varying distance from the equator.<br/>
Output can be found [output_WeatherPy](https://github.com/Ash-Tao/python_api_challenge/tree/main/output_WeatherPy)<br/>
- Create a series of scatter plots to showcase the following relationships:<br/>
  * __Temperature (F) vs. Latitude__<br/>
The equator has the highest temperature, and the temperature gradually decreases as it moves along the equator towards the earth's poles.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Latitude%20vs.%20Temperature%20(Max).png" width="500"><br/>
  * __Humidity (%) vs. Latitude__<br/>
There is no obvious correlation between the two variables.<br/>
But, when the latitude is between 0 to 20, the humidity is the lowest.<br/>
Afterwards, as the latitude moves to the sides, the humidity gradually increases.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Latitude%20vs.%20Humidity.png" width="500"><br/>
  * __Cloudiness (%) vs. Latitude__<br/>
There is no obvious correlation between the two variables.<br/>
But cloud cover appears to be centered around 0% and 100%.<br/>
And in the middle part, the plot has a certain concentration in the 20%, 40% and 75% parts.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Latitude%20vs.%20Cloudiness.png" width="500"><br/>
  * __Wind Speed (mph) vs. Latitude__<br/>
There is no obvious correlation between the two variables.<br/>
But for most cities, they have wind speeds between 0-20 mph.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Latitude%20vs.%20Wind%20Speed.png" width="500"><br/>

- Create separate plots -linear regression into Northern Hemisphere(0 to 90)  and Southern Hemisphere(-90 to 0) :<br/>
Related information for R-Value in Linear Regression.<br/>
Typically:<br/>
1.0 = |R| - Perfect positive/negative correlation<br/>
0.8 <= |R| < 1.0 - Very strong positive/negative correlated.<br/>
0.6 <= |R| < 0.8 - Strong positive/negative correlated.<br/>
0.4 <= |R| < 0.6 - Moderate positive/negative correlated.<br/>
0.2 <= |R| < 0.4 - Weak positive/negative correlated.<br/>
0.0 < |R| < 0.2 - Very weak positive/negative correlated.<br/>
0.0 = |R| - No correlated.<br/>
  * __Northern Hemisphere - Temperature (F) vs. Latitude__<br/>
The R-value between these two variables is -0.89, which means that there is a very strong negative correlation between Max Temp Latitude in the Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Northern%20Hemisphere%20-%20Max%20Temp%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Southern Hemisphere - Temperature (F) vs. Latitude__<br/>
The R-value between these two variables is 0.50, which means that there is a moderate positive correlation between Max Temp and Latitude in the Southern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Southern%20Hemisphere%20-%20Max%20Temp%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Northern Hemisphere - Humidity (%) vs. Latitude__<br/>
The R-value between these two variables is 0.30, which means that there is a weak positive correlation between Humidity and Latitude in the Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Northern%20Hemisphere%20-%20Humidity%20(%25)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Southern Hemisphere - Humidity (%) vs. Latitude__<br/>
The R-value between these two variables is 0.36, which means a weak positive correlation between Humidity and Latitude in the Southern Hemisphere. And it is even weaker in Southern Hemisphere than it is in Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Southern%20Hemisphere%20-%20Humidity%20(%25)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Northern Hemisphere - Cloudiness (%) vs. Latitude__<br/>
The R-value between these two variables is 0.17, which means that there is a very weak positive correlation between Cloudiness and Latitude in the Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Northern%20Hemisphere%20-%20Cloudiness%20(%25)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Southern Hemisphere - Cloudiness (%) vs. Latitude__<br/>
The R-value between these two variables is 0.35, which means that there is a weak positive correlation between Cloudiness and Latitude in the Southern Hemisphere. And it is stronger in Southern Hemisphere than it is in Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Sorthern%20Hemisphere%20-%20Cloudiness%20(%25)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Northern Hemisphere - Wind Speed (mph) vs. Latitude__<br/>
The R-value between these two variables is 0.11, which means that there is a very weak positive correlation between Wind Speed and Latitude in the Northern Hemisphere.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Northern%20Hemisphere%20-%20Wind%20Speed%20(mph)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>
  * __Southern Hemisphere - Wind Speed (mph) vs. Latitude__<br/>
The R-value between these two variables is -0.39, which means that there is a weak negative correlation between Wind Speed and Latitude in the Southern Hemisphere. And it is stronger in Southern Hemisphere than it is in Northern Hemisphere. But the linear regression goes to the opposite direction, negative instead of positive.<br/>
  <img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_WeatherPy/Southern%20Hemisphere%20-%20Wind%20Speed%20(mph)%20vs.%20Latitude%20Linear%20Regression.png" width="500"><br/>


### Task 2: VacationPy
Create a heatmap showing the humidity for each city in Task 1. Mark several hotel locations on this heatmap.<br/>
Output can be found [output_VacationPy](https://github.com/Ash-Tao/python_api_challenge/tree/main/output_VacationPy)<br/>
* Create a heatmap showing the humidity of the reduced DataFrame from Part 1 after filtering cities based on certain criteria.<br/>
<img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_VacationPy/Heat%20Map.png" width="600"><br/>
  * A max temperature lower than 80 degrees but higher than 70.
  * Wind speed less than 10 mph.
  * Zero cloudiness.
  * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

* Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.
Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**。
<img src="https://github.com/Ash-Tao/python_api_challenge/blob/main/output_VacationPy/Heat%20Map%20with%20Hotel.png" width="600"><br/>

* **Hint:** Consider the full range of latitudes.
Since the number of cities in the northern and southern hemispheres is different, in order to get an equal amount of cities as possible in both hemispheres. I used a loop to control the number of cities in the stage of getting city list, 270 for both hemispheres.
