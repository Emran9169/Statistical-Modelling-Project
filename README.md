# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This project aims to analyze bike-sharing data in New York City using the CityBikes, Foursquare, and Yelp APIs. The primary goals include:

1. Understanding the distribution and utilization of bike-sharing stations in New York City.
2. Comparing the coverage and data quality of the Foursquare and Yelp APIs regarding local points of interest (POIs) near bike stations.
3. Building a statistical model to explore the relationship between the availability of bikes at these stations and the characteristics of nearby POIs.

## Process
1. Data Collection: Connected to the CityBikes API to retrieve data on bike stations in New York, focusing on their locations and the number of available bikes and empty slots.
2. API Integration and Comparison: Using the latitude and longtiude of citybike API i was able to integrate it with Foursquare and Yelp APIs to gather data. 
I got number of public transportation, number of chinese restaurant and number of sport recreation facilities from Foursquare API across each bike station.
In the case of Yelp API, I extracted a data about number of chinese restaurant around each bike station inorder to compare it with the one I got from Foursquare.
3. Conducted a comparative analysis of the data quality and coverage provided by these APIs.
4. Data Analysis and Visualization: Analyzed the collected data and used visualizations like heatmaps and scatter plots to explore correlations and patterns.
5. Statistical Modelling: Developed a regression model using Python's statsmodels module to understand the relationship between bike availability and POI characteristics.

## Results
The comparison of Foursquare and Yelp APIs revealed that Yelp reported a higher average number of Chinese restaurants near bike stations than Foursquare, which was an unexpected finding. I was able to determine in the data visualization step as there is no a clear trend between free_bikes and the POI's. The statistical regression model indicated a moderate correlation between bike availability and factors like nearby public transportation and restaurants, explaining approximately 17.9% of the variance in free bike availability. The presence of public transportation options and Chinese restaurants positively correlated with the availability of free bikes, while the number of empty slots showed a negative correlation and number of sport recreation facilities showed no correlation at all.

## Challenges 
1. API Limitations: Both Foursquare and Yelp APIs had limitations on the number of responses per call, which restricted the depth of data that could be gathered.
2. Yelp API Restrictions: Yelp's daily limit on API calls is 500 which affected my data to contain only 500, although i got 2167 bike station in NewYork, i was obliged to use the first 500 bike station for my dataset.r
Data Integration and Analysis Complexity: Merging data from multiple sources and ensuring accurate analysis required careful data handling and sophisticated statistical techniques.

## Future Goals
1. Expanding Data Sources: Incorporating additional data sources, such as traffic and weather data, to gain more comprehensive insights into bike-sharing patterns.
Integrating real-time data can provide insights into how traffic conditions and weather impact bike-sharing usage. For instance, understanding the effect of rush hour traffic or rainy weather on bike availability can help on building a better bike usage pattern.
3. Broader Geographic Scope: Extending the analysis to additional cities or even a country-wide scale to compare bike-sharing trends and patterns in different urban environments.
