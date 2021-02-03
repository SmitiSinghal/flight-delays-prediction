# Predicting Flight Delays and Cancellations using Decision Tree
## About the project - 
Problem Statement - To build a machine learning model for predicting flight delays and cancellations based on the patterns in dataset. The dataset consists of tabular data consisting of 31 columns.

### Dataset Link - 
https://www.kaggle.com/usdot/flight-delays

### Features of dataset-
|    |       Feature       | Datatype |                                                 Description                                                |
|----|:-------------------:|:--------:|:----------------------------------------------------------------------------------------------------------:|
| 0  | YEAR                | int64    | Year of the flight trip                                                                                    |
| 1  | MONTH               | int64    | Month of the flight trip                                                                                   |
| 2  | DAY                 | int64    | Date of the flight trip                                                                                    |
| 3  | DAY_OF_WEEK         | int64    | Day of Week of the flight trip (from 1 to 7)                                                               |
| 4  | AIRLINE             | object   | Airline identifier                                                                                         |
| 5  | FLIGHT_NUMBER       | int64    | Flight identifier                                                                                          |
| 6  | TAIL_NUMBER         | object   | Aircraft identifier                                                                                        |
| 7  | ORIGIN_AIRPORT      | object   | Starting airport                                                                                           |
| 8  | DESTINATION_AIRPORT | object   | Destination airport                                                                                        |
| 9  | SCHEDULED_DEPARTURE | int64    | Planned departure time                                                                                     |
| 10 | DEPARTURE_TIME      | float64  | WHEEL_OFF - TAXI_OUT                                                                                       |
| 11 | DEPARTURE_DELAY     | float64  | Total delay on departure                                                                                   |
| 12 | TAXI_OUT            | float64  | The time duration elapsed between departure from the origin airport gate and wheels off                    |
| 13 | WHEELS_OFF          | float64  | The time point that the aircraft's wheels leave the ground                                                 |
| 14 | SCHEDULED_TIME      | float64  | Planned time amount needed for the flight trip                                                             |
| 15 | ELAPSED_TIME        | float64  | AIR_TIME+TAXI_IN+TAXI_OUT                                                                                  |
| 16 | AIR_TIME            | float64  | The time duration between wheels_off and wheels_on time                                                    |
| 17 | DISTANCE            | int64    | Distance between two airports                                                                              |
| 18 | WHEELS_ON           | float64  | The time point that the aircraft's wheels touch on the ground                                              |
| 19 | TAXI_IN             | float64  | The time duration elapsed between wheels-on and gate arrival at the destination airport                    |
| 20 | SCHEDULED_ARRIVAL   | int64    | Planned arrival time                                                                                       |
| 21 | ARRIVAL_TIME        | float64  | WHEELS_ON+TAXI_IN                                                                                          |
| 22 | ARRIVAL_DELAY       | float64  | ARRIVAL_TIME-SCHEDULED_ARRIVAL                                                                             |
| 23 | DIVERTED            | int64    | Aircraft landed on airport that out of schedule                                                            |
| 24 | CANCELLED           | int64    | Flight Cancelled (1 = cancelled)                                                                           |
| 25 | CANCELLATION_REASON | object   | Reason for Cancellation of flight: A - Airline/Carrier; B - Weather; C - National Air System; D - Security |
| 26 | AIR_SYSTEM_DELAY    | float64  | Delay caused by air system                                                                                 |
| 27 | SECURITY_DELAY      | float64  | Delay caused by security                                                                                   |
| 28 | AIRLINE_DELAY       | float64  | Delay caused by airline                                                                                    |
| 29 | LATE_AIRCRAFT_DELAY | float64  | Delay caused by aircraft                                                                                   |
| 30 | WEATHER_DELAY       | float64  | Delay caused by weather                                                                                    |
### The notebook includes :
- Data Cleaning and Visualization
- Prediction using Decision Tree 
- Evaluating the model with auc score