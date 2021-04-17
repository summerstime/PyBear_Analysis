# PyBear Analysis

Module 5 Project

## Overview

This project is to satisfy the requirements for the fifth module challenge in the Data Analysis Bootcamp.
In this project we have landed a job with PyBer, a python based ride share company. V. Isualize has given
an assignment to create a summary DataFrame of the ride-sharing data by city type. Also included in the project
is to create a line chart displaying the three types of city types, Urban, Suburban, and Rural.  

## Results

* The summary of the evaluation is...
![PyBer Summary](https://github.com/summerstime/PyBer_Analysis/blob/main/Resources/PyBer_Summary.png)

Rural city types have the lowest number of rides at 125 and drivers at 78; but the highest average fares at $34.62 for rides and $55.49 for drivers.
Suburban city types are across the middle for all aspects, total numbers and average fares, with rides (625), drivers (490), average fare/ride ($30.97), and average fare/driver ($39.50).
Urban city types have the largest number of rides at 1,625 with 2,405 drivers; but the lowest average fares at $24.53 per ride and $16.57 per driver.

### Charting the Data
![PyBer Summary Chart](https://github.com/summerstime/PyBer_Analysis/blob/main/Analysis/PyBer_Summary_Chart.png)


## Summary
In summary, the results for the three city types show an expected supply and demand outcome. Urban cities have more riders and drivers, which drives the fares down. 
There's more competition, so getting the fare is more challenging from the driver's point of view. The opposite is true for rural city types. The rider is somewhat limited
by the number of drivers available in the area. People in rural areas typically drive themselves.

* Create a program for rural areas that focuses on getting seniors to their doctors appointments or run errands for them.
* Create a program for suburban areas that helps families get the kids where they need to be. Help the parents meet the kids at the destination.
* Create a program for urban areas that focuses on safe drivers for parties and bars. Drivers ready to get the drinkers off out from behind the wheel.   

## Analysis Details
The analysis started with two data sets that were joined into one dataframe. This data was then grouped, resampled, and plotted.
One of the main problems experienced in this challenge was the differing output of the pivot.loc['1/1/2019':'4/29/2019']. 

This date range produced this output. 
![PyBer Summary Chart](https://github.com/summerstime/PyBer_Analysis/blob/main/Analysis/PyBer_Summary_Chart2.png)

Reviewing the CSV file, showed that several days of data were missing, which caused the first part of April to dip for all city types.
Changing the date to be in May, brought the April data back. So the final line chart include the month of May.

Requested a TA to take a look and it was not clear to either of us why the data was disappearing. 
Changing the dates to see different outcomes, it showed that April was not special in this and would change the particular week of data it affected.