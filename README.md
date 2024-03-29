# Weather Data Trip Analysis

## Purpose
The purpose of this project is to develop a PlanMyTrip app that will identify travel destinations and hotels based on user input of weather preferences. From the list of potential destinations, the tester can choose 4 cities to create a travel itenerary and using the Google Maps Directions API, a travel route is created between the four cities, as well as a marker layer map.

## Technology Used

![download](https://user-images.githubusercontent.com/98500639/185665121-0e830c15-e612-487d-92e5-a0c63696e19a.png)
![download](https://user-images.githubusercontent.com/98500639/185665197-583520c3-840b-4187-a5ea-ede9e925c473.png)
![download](https://user-images.githubusercontent.com/98500639/185665270-c06415c7-356d-4748-98be-e713c48a1a7b.png)
![download](https://user-images.githubusercontent.com/98500639/185665469-27eabbcd-f5d2-4ea6-b9e6-ca1ea3e079a4.png)

## Tasks

Three main tasks were needed to complete this project. 

### 1) Weather data is retrieved. 

#### Approach
A set of 2000 random latitudes and longitudes is generated and the nearest city is retrieved. Then, An API call is performed with the OpenWeatherMap. Information retrieved from the API call includes: Lat/Long, Max Temp, Percent Humidity, Percent Cloudiness, Wind Speed, Weather Descriptions. This weather data is added to a DataFrame. A sample of the first 5 rows and what this dataframe looks like is below.

![DataFrame](https://github.com/JeremyKRay/Weather_Data/blob/f5c0f224ab79c7f6eb432494b1c624cc478db32e/Weather%20DataFrame.png)

### 2) A customer Travel Destinations Map is created. 

#### Approach
Input statements are created that prompt the user to enter their minimum and maximum temperature criteria for their vacation. The loc method is used to filter the DataFrame for temperature criteria collected. The hotell_df dataframe is used to find nearest hotels based on cities found from the search parameters. The marker layer map code is updated to create pop-up markers for each city on the map. The map can be seen below.

![Vacation Map](https://github.com/JeremyKRay/Weather_Data/blob/075f5964ce81f0e6d2cc4305740750d9f75b8a74/WeatherPy_vacation_map.png)

### 3) A travel itenerary map is created.

#### Approach
Finally, the Google Directions API is used to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, a marker layer map is created with a pop-up marker for each city on the itinerary. The locations and their pop-up markers are shown below.

![Itenerary Markers](https://github.com/JeremyKRay/Weather_Data/blob/7262a4e0d278403966cc5e8cd30b9ebeb44afd05/WeatherPy_travel_map.png)

## Results

A snapshot of the final itenerary map with the locations and the route highlighted is shown below.

![Route Itenerary](https://github.com/JeremyKRay/Weather_Data/blob/22759c704a3bc613ce5a8aaa14d8f3939d7454df/WeatherPy_travel_map_markers.png)
