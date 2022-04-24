# World_Weather_Analysis
Analysis of 2000 randomly generated coordinate pairs for city location and weather conditions for development of user input responsive travel plans. The user input will generate a list of cities that mean desired weather conditions and generate an output with nearby hotels, as well as give details for travel times before multiple cities if desired. 

##**Resources**
Data Sources: cities.csv
Software: Python 3.9.7, Jupyter Notebook 6.4.0, GMAPS API, OpenWeatherMap API

##**Overview**
To aid in the creation and beta testing of an app that takes user input to plan trips, creation of a list of random cities and input boxes for desired destination temperatures were created to generate a customized list of travel destination. From this information, gmaps figures were created with the perferred destination list were added to include desired information, such as maximum temperature, humidity, cloudiness percentage, and current weather conditions. Additionally, gmaps figures were created to show travel between multiple desired cities to give beta tester as many option as possible when planning their perfect vacation through the app. This figure displays all previous desired information in pop-up boxes, as well as driving routes, and time to travel between destinations.

##**Results** 
The original database used for additionally preferentially selection was created with 2000 random numbers and citipy was used to find cities close to the coordinates generated. This resulted in a master list of 742 cities to choose parameters for(available in Weather_Database folder, in the WeatherPy_Database.csv). From this list user input for desired minimum and maximum temperature, and GMAPS API was used to find hotels within a 5k meter radius, the data was cleaned through dropping any rows with null values(available in Vacation_Search folder, in the WeatherPy_vacation.csv). The resulting database is shown below. 


![cleaned_hotel_df](https://user-images.githubusercontent.com/100040705/164981867-9b63b92f-48b1-45d3-b74a-4db18fd94bfb.png)

With this information, a GMAPS figure was created showing markers for all locations with hotels nearby within the users search parameters. Pop up boxes were created to show desired information, city & country name, current weather description, and maximum temperature for the city. The figure created is as shown below. 

![preferred_cities_gmaps_labeled](https://user-images.githubusercontent.com/100040705/164981966-ca385fb7-c4e2-471c-88de-58e3bb185077.png)


An additional map was created to show the route between four cities so users can see travel options and get directions and travel times. The resulting figure is as shown below. The same pop up markers are available in this map as well. 


![preferred_cities_gmaps_labeled](https://user-images.githubusercontent.com/100040705/164982670-4060c939-6519-4ad1-9d40-408dec57068b.png)

##**Summary**
Based on input received from beta testers, the travel app was updated to be more interactive, allowing user selection of desired weather conditions and filtering a master list so the results are tailored to users needs. These selections were then used to show all travel destinations with hotels and weather conditions for user selection. Travel routes and times between desired cities is shown through maps, allowing users to have many options when planning their itinerary. Highly interactive applications allow ease of use for users and create the most streamlined experience possible, allow drives in profit and customer satisfaction. These application updates will be used for future beta testing, and could be refactored to futher tailer to user parameters. 

