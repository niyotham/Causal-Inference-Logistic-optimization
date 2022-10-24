# Delivery drivers location optimization with Causal Inference
## Introduction
Work  on clients’ data to help it understand the primary causes of unfulfilled requests as well as come up with solutions that recommend drivers locations that increase the fraction of complete orders. 

## Business overview


## objective

Work  on clients’ data to help client understand the primary causes of unfulfilled requests as well as come up with solutions that recommend drivers locations that increase the fraction of complete orders. Since drivers are paid based on the number of requests they accept, the solution will help client business grow both in terms of client satisfaction and increased business. 

## Data Cleaning
 Drop columns with empty entries
 Drop rows with NaN entries
 Merge the Two tables
## Feature Engineering
 > Generate month, day, week day, and an hour from the trip start time column.
 - Calculate the driver proximity to the order using trip origin and driver location when the driver got the order which is given in lat and lng in the second table.
 - Calculate trip distance and trip duration and then trip speed.
-  [x]I also used the API from https://api.weatherbit.io/v2.0/history/daily? to get the weather at a given location and time-stamp.
 Public, school, regional and national holidays are calculated from the trip start time.
## Visualization
 * plot driver distance vs acceptance rate
 * plot latitude vs longitude of dirver location
## Causal Inference
## Conclusion
## Future Works
