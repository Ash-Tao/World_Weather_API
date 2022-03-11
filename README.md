# python_api_challenge

## Task 1: WeatherPy
Visualize the weather of 500+ cities of varying distance from the equator.<br/>
Tools: *[simple Python library](https://pypi.python.org/pypi/citipy)*, *[OpenWeatherMap API](https://openweathermap.org/api)*.
### Targets
- Create a series of scatter plots to showcase the following relationships:
  * Temperature (F) vs. Latitude
  * Humidity (%) vs. Latitude
  * Cloudiness (%) vs. Latitude
  * Wind Speed (mph) vs. Latitude
  After each plot, add a sentence or two explaining what the code is analyzing.

Create separate plots -linear regression into Northern Hemisphere(0 to 90)  and Southern Hemisphere(-90 to 0) :
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude
describe any relationships that you notice and any other findings you may have.



### Part 2: VacationPy

Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.

* **Note:** Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out [Google Maps Platform Billing](https://developers.google.com/maps/billing/gmp-billing#monitor-and-restrict-consumption) and [Manage your cost of use](https://developers.google.com/maps/documentation/javascript/usage-and-billing#set-caps) for more information.

* **Note:** If you are having trouble displaying the maps, run `jupyter nbextension enable --py gmaps` in your environment and then retry.

To complete this part of the assignment, you will need to do the following:

* Create a heat map that displays the humidity for every city from Part 1, as in the following image:

  ![heatmap](Images/heatmap.png)

* Narrow down the DataFrame to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

  * **Note:** Feel free to adjust your specifications, but make sure to limit the number of rows returned by your API requests to a reasonable number.

* Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**, as in the following image:

  ![hotel map](Images/hotel_map.png)

As final considerations:

* You must complete your analysis using a Jupyter notebook.
* You must use the Matplotlib or Pandas plotting libraries.
* For Part 1, you must include a written description of three observable trends based on the data.
* For Part 2, you must take a screenshot of the heatmap that you create and include it in your submission.
* Your plots must include labeling aspects like plot title (with date of analysis) and axis labels.
* For max intensity in the heatmap, try setting it to the highest humidity found in the dataset.

## Hints and Considerations

* The city data that you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.

* If you'd like a refresher on the geographic coordinate system, [this site](http://desktop.arcgis.com/en/arcmap/10.3/guide-books/map-projections/about-geographic-coordinate-systems.htm) has great information.

* Next, take some time to study the OpenWeatherMap API. Based on your initial study, you should be able to answer basic questions about the API: Where do you request the API key? Which Weather API in particular will you need? What URL endpoints does it expect? What JSON structure does it respond with? Before you write a line of code, you should have a crystal-clear understanding of your intended outcome.

* A starter code for citipy has been provided. However, if you're craving an extra challenge, push yourself to learn how it works: [citipy Python library](https://pypi.python.org/pypi/citipy). Before you try to incorporate the library in your analysis, start with simple test cases outside your main script to confirm that you are using it correctly. Often, when introduced to a new library, students will spend hours trying to figure out errors in their code&mdash;a simple test case can save you a lot of time and frustration.

* You will need to apply your critical thinking skills to understand how and why we're recommending the tools we are. What is citipy used for? Why would you use it in conjunction with the OpenWeatherMap API? How would you do so?

* While building your script, pay attention to the cities you are using in your query pool. Are you covering the full range of latitudes and longitudes? Or are you choosing 500 cities from one region of the world? Even if you were a geography genius, simply listing 500 cities based on your personal selection would create a biased dataset. Try to think of ways that you can counter this. 

  * **Hint:** Consider the full range of latitudes.

* Once you have computed the linear regression for one relationship, you will follow a similar process for all other charts. As a bonus, try to create a function that will create these charts based on different parameters.

* Remember that each coordinate will trigger a separate call to the Google API. If you're creating your own criteria to plan your vacation, try to reduce the results in your DataFrame to 10 or fewer cities.

* Ensure your repository has regular commits and a thorough README.md file.

* Lastly, remember that this is a challenging activity. Push yourself! If you complete this task, you can safely say that you've gained a strong understanding of the core foundations of data analytics, and it will only get better from here. Good luck!

## Rubric

[Unit 6 Homework Rubric](https://docs.google.com/document/d/1Y17QYjs0KMeEPPGd_1BpMjnqXiTaJVeFwqea5ReMdeU/edit?usp=sharing)

- - -

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
