# Zuber

In this project I analyzed Zuber, a new ride-sharing company being launched in Chicago. My task is to find patterns in the information available. To understand passenger preferences and the impact of external factors on rides.
Working with a database, I analyzed data from competitors and tested a hypothesis about the impact of weather on trip frequency.


**Data description (SQL)**

A database with information on cab rides in Chicago:
* neighborhoods table: data on the city's neighborhoods
* name: name of the neighborhood
* neighborhood_id: neighborhood code
* cabs table: data on cabs
* cab_id: vehicle code
* vehicle_id: the technical identification of the vehicle
* company_name: the company that owns the vehicle
* trips table: data on rides
* trip_id: trip code
* cab_id: code of the vehicle operating the run
* start_ts: date and time of the start of the run (time rounded to the hour)
* end_ts: date and time of the end of the race (time rounded to the hour)
* duration_seconds: race duration in seconds
* distance_miles: distance covered in miles
* pickup_location_id: pickup neighborhood code
* dropoff_location_id: delivery neighborhood code
* weather_records table: weather data
* record_id: weather record code
* ts: records date and time (time rounded to the hour)
* temperature: temperature when the record was made
* description: brief description of the weather conditions, e.g. "light rain" or "sparse clouds"

**Python**

You now have these two CSVs:
project_sql_result_01.csv. 

**It contains the following data**
* company_name: name of the cab company
* trips_amount: the number of runs for each cab company from November 15 to 16, 2017.

project_sql_result_04.csv. 
**It contains the following data**
* dropoff_location_name: Chicago neighborhoods where the runs ended
* average_trips: the average number of trips that ended in each neighborhood in November 2017.


Test the hypothesis: "The average length of rides from the Loop to O'Hare International Airport changes on rainy Saturdays."

**Conclusion**
Passenger preferences are:
1- Loop 2- River North 3- Streeterville 4- West Loop 5- O'Hare 6- Lake View 7- Grant Park 8- Museum Campus 9- Gold Coast 10- Sheffield & DePaul

External factors do have an impact, both on the length of journeys (proven in the statistical test) and on the number of runs (difference in rows of the dataframe filtered by good weather (888) and bad weather (180). With a total of 708 more runs on days with good weather).
