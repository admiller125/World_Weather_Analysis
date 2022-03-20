# World_Weather_Analysis

## Overview of Analysis
The purpose of this project is to use apis to determine a list of random vacation destinations that meet travel criteria.

### Summary and Results
The first step was to generate a list of random cities to analyze. 2000 random coordinates were generated and then citipy was used to find the nearest city to the coordinates provided. Then I retrieved data from the OpenWeatherMap api 
and organized it into a dataframe and wrote the information to a csv to use as my database. Then the data was filtered based on the "Max Temp" value which was inputed to not exceed 90F and not go below 70F. I then used the google 
geocoding api to find the nearest hotel to the randomly generated cities in the requested "Max Temp" range. Then the values associated with the hotels found were written to a csv. The hotels along with their city, country, and current 
weather description was formatted and placed on a google map as shown below.

![](Vacation_Search/WeatherPy_vacation_map.png)

Then the google "Directions API" was used to find the path between four chosen hotels. Below is the directions layer map created as a result.

![](Vacation_Itinerary/WeatherPy_travel_map.png)

Finally, the information regarding the four hotel locations into markers that displayed the hotel name, city, county, and current weather description.

![](Vacation_Itinerary/WeatherPy_travel_map_markers.png)




 