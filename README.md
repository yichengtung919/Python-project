# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Integrating with multiple APIs, organizing the data retrieved from these APIs, and then using that data for statistical modeling.

## Process
### First start by exploring the city bikes api to obtain information on bike stations within a city(Vancouver). 
### Send calls to foursquare API using the coordinates of the bike stations to obtain points of interests such as restaurants and grocery stores.
### Replicate the process and send requests to Yelp API. 
### Combine the citybike data and the POI dataset for our final regression model.


## Results
The r-squared is very low at .001 which mean it can only explain .1 % of the dataset. The p value here shows .68 which indicates that it is not statistically significant. Overall this is not a good model to predict the number of bikes based on number of restaurants nearby. Same with the data using grocery store data, the model does not fit well and is not statistically significant.

## Challenges 
Since bike station and restaurant datasets contain different columns and there are no common data points, it didn't make sense to left join the datasets, because we are only getting the bike station dataset with additional columns that fills with Nan values. After dropping all the Nan values we ended up with an empty dataset. So it has been difficult to join datasets from different API.
Additon: EDA and data cleaning is done throughout different sections whenever a dataset is requested from the APIs. However, it seem like documentation is a challenge to convey the thought process and organize it in a sequential way. I have tried to highlight them with subsections so hopefully they can be identified more easliy.

## Future Goals
Explore more on the datasets and find more relationship between bike station data and POIs. By adding more independent variables there could be a chance of having a model that better predicts the dependant variable.  
