# Ride-Sharing Data Analysis

## Overview
The purpose of this project was to analyze and compare ride-sharing data for urban, suburban, and rural cities. The analysis examined total rides, total drivers, total fares, average fare per ride, and average fare per driver for each city type. Total weekly fares for urban, suburban, and rural cities over a period of four months (January – April 2019) were visualized in a single line graph to facilitate easy comparison of fares among the three city types. The analysis will be used by the ride-sharing company’s leadership to inform business decisions.

## Results
All analysis for this project was performed using [city](Resources/city_data.csv) and [ride](Resources/ride_data.csv) datasets. A [Python script using Pandas in Jupyter Notebook]( PyBer_Challenge.ipynb) was developed to clean and merge the datasets, analyze the data, and create graphs to visualize the data.

As shown in the DataFrame image below, urban cities combined had the highest numbers for total rides, total drivers, and total fares, followed by suburban cities and then rural cities with the lowest numbers. 
-    The total number of rides for urban cities was about two and a half times the number for suburban cities and 13 times the number for rural cities. 
-    There were nearly five times as many total drivers for urban cities as for suburban cities and nearly 31 times as many for urban cities as for rural cities.
-    The total fares earned for urban cities was about double that of suburban cities and about nine times that of rural cities.

With respect to average fare per ride and average fare per driver, both were highest for rural cities, followed by suburban cities and then urban cities with the lowest average fare per ride and average fare per driver. The difference among city types was greater for average fare per driver than for average fare per ride.
-    The average fare per driver for rural cities was about 40% higher than that of suburban cities and about 235% higher than that of urban cities.  
-    The average fare per driver for rural cities was only about 12% higher than that of suburban cities and about 41% higher than that of urban cities.

![img1](Resources/City_Type_Comparison_Table.png)


The graph below of total weekly fares by city type over the period from January through April 2019 shows that urban cities had the highest weekly total fares, followed by suburban cities and then rural cities. All three city types experienced variability in total fares from week to week, with urban cities having the greatest range of total weekly fares (from a low of about $1,662 to a high of about $2,471) and rural cities having the smallest range (from a low of about $68 to a high of about $501). All three city types shared a week of higher total fares in late February, but other high points differed more among city types.

![img2](Resources/Pyber_fare_summary.png)


## Summary
Based on the analysis outlined above, below are recommendations for the ride-sharing company and its CEO.
1.    Urban cities had more total drivers than they did total rides during the period covered by these data. Suburban and rural cities had more total rides than total drivers, but the ratio of rides to drivers was still very low (1.3 and 1.6, respectively). These numbers suggest that not all drivers included in the total driver counts were actively providing rides during the period. The company should attempt to include only active drivers in the driver counts in order to have more meaningful analysis of disparities among city types, especially with respect to average fares per driver.
2.    Urban cities clearly make up the ride-sharing company’s largest market, but the number of drivers in urban cities is too high relative to the demand for rides (for example, there are 31 times as many drivers in urban cities compared with rural ones, but only 13 times as many rides and nine times as much earned in total fares). This results in a much lower average fare earned per driver in urban cities than in rural ones (and to a lesser extent suburban ones). Depending on the findings of the additional analysis suggested above, the CEO should consider measures to shift the distribution of drivers among city types to be more in proportion to demand. This would make the competition among drivers for rides more similar across city types and reduce disparities in average fares.
3.    The dataset lacks data on ride length, which could provide useful context to the consideration of average fare per ride. It is possible that the average fare per ride in urban cities is less than in suburban and especially rural ones because ride times and distances may be shorter in urban areas than in suburban and rural ones where points of interest are typically more spread out. The company should attempt to include data on ride times and ride distances in order to calculate average fare per minute and average fare per mile. This analysis would be a useful supplement to the comparison of average fares per ride among city types and should be considered in the CEO’s decision-making.
