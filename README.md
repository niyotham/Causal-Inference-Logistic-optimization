# Logistic optimization: Delivery drivers location optimization with Causal Inference
## Introduction
Work  on clients’ data to help it understand the primary causes of unfulfilled requests as well as come up with solutions that recommend drivers locations that increase the fraction of complete orders. 

## Business overview
We will try to answer some interesting question that cannot be answered by just analyzing observational data alone.

### These questions can be similar to:

• Given drivers are recommended to move 1km every 30 mins in a selected direction, what happens to the number of unfulfilled requests?

• If we assume we know the location of the next 20% of orders within 5km accuracy, what happens to the number of unfulfilled requests?

• Had we changed the time requirements to drivers operating time in the past, what fractions of orders could have been completed?

• If I increased the number of drivers by 10% cumulative per month, what fraction of orders can be completed?


## objective

Work  on clients’ data to help client understand the primary causes of unfulfilled requests as well as come up with solutions that recommend drivers locations that increase the fraction of complete orders. Since drivers are paid based on the number of requests they accept, the solution will help client business grow both in terms of client satisfaction and increased business. 

## Data Cleaning
- [x] Drop columns with empty entries
 - [x] Drop rows with NaN entries
- [x]  Merge the Two tables
## Feature Engineering
- [x] Generate month, day, week day, and an hour from the trip start time column.
- [x] Calculate the driver proximity to the order using trip origin and driver location when the driver got the order which is given in lat and lng in the second table.
 - [x] Calculate trip distance and trip duration and then trip speed.
- [x] I also used the API from https://api.weatherbit.io/v2.0/history/daily? to get the weather at a given location and time-stamp.
 Public, school, regional and national holidays are calculated from the trip start time.
## Visualization
 - [x]  plot driver distance vs acceptance rate
 - [x]  plot latitude vs longitude of dirver location
## Causal Inference
- [x] Used [causalnex libary](https://causalnex.readthedocs.io/en/latest/03_tutorial/01_first_tutorial.html) to build structural model
- [x] generarated some graphs
## Folder Structure

###  maps
 - [x] generated maps screenshots from this project  are found here
 
 ###  screenshots
 Folder caointing information about structural model of the causalnex network and visualization

### notebooks
Caintains separate notebooks for the following purposes:

 - [x] EDA on  separate datsets 
 - [x] EDA on merged two dasets 
  - [x]  EDA and feature engineering on merged datasets.
 - [x] Causal Inference and Causal Graphs
Some screenshots from the EDA
Locations of origin for requests

## Conclusion
## Future Works
