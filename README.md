# Weather Data Trip Analysis

## Purpose
The purpose of this project is to develop a PlanMyTrip app that will identify travel destinations and hotels based on user input of weather preferences. From the list of potential destinations, the tester can choose 4 cities to create a travel itenerary and using the Google Maps Directions API, a travel route is created between the four cities, as well as a marker layer map.

## Tasks

Three main tasks were needed to complete this project. 

1) Weather data is retrieved. 

### Approach
A set of 2000 random latitudes and longitudes is generated and the nearest city is retrieved. Then, An API call is performed with the OpenWeatherMap. Information retrieved from the API call includes: Lat/Long, Max Temp, Percent Humidity, Percent Cloudiness, Wind Speed, Weather Descriptions. This weather data is added to a DataFrame. A sample of the first 5 rows and what this dataframe looks like is below.

![DataFrame](https://github.com/JeremyKRay/Weather_Data/blob/f5c0f224ab79c7f6eb432494b1c624cc478db32e/Weather%20DataFrame.png)

2) A customer Travel Destinations Map is created. 

### Approach
Input statements are created that prompt the user to enter their minimum and maximum temperature criteria for their vacation. The loc method is used to filter the DataFrame for temperature criteria collected. The hotell_df dataframe is used to find nearest hotels based on cities found from the search parameters. The marker layer map code is updated to create pop-up markers for each city on the map. The map can be seen below.

3) A travel itenerary map is created.

### Approach
Finally, the Google Directions API is used to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, a marker layer map is created with a pop-up marker for each city on the itinerary. 

## Results
A snapshot of the final itenerary map is shown below.
