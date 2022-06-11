# Ford GoBike Data investigation
## by (Omnia Imam)


## Dataset

> This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area in fabuary 2018. 
The dataset includes:
* an ID number for each bicycle
* how long it was rented for, in seconds
* the beginning and end staton ID, latitude, longitude and station name
* the start and end time
* the year the user was born
* the gender of the user
* bike_share_for_all_trip
* whether the user has a subscription to the service or not

> There are 183412 rows and 16 columns.

> There was some cleaning done to the dataset. This included: 
* Deleting the rows without gender or birth year, and dropping some unneeded columns containing null values.
* Only use ages that are reasonable. Check for abnormally old or young values and remove them,and ages older than 100 were removed from the data
* Change data types; times to datetimes.
* Extract days of the week from start_time

## Summary of Findings

- The proportion  of male users is the hieghest , followed by females, then others.
- The majority of the users are subscribers (90.5% of users are subscribers and 9.5% customers)
- The mean age of the members is 34 years old and number of members decreases as age goes higher.

- The majority of the ride are less than 20 minutes,with average time duration of 11.49 minutes.
- The majority of rides are on thursday then tuesday followed by wednesday,friday and Monday, While having Saturday and Sunday of the least reservation frequencies. When analyzing the daily usage for both types of users seperatly we find that "Thursday" is still the most frequent day of reserving rides for both types, followed by "Friday" for customers, and "Tuesday" for subscribers. 
- A larger percentage of customers are taking longer rides duration compared to subscripers 


## Key Insights for Presentation

> For my presentation, I will focus on the difference in usage for customers and subscribers, and how long does the average trip take(which are my main features of interest). I will first show the univariate results, such as the distribution of different variables like (gender,user type,duaration,age) and usage on days of the week. then we will continue by adding more variables in bivariate and multivariate visuals to see the relationship between different variables. 
> My conclusion is that: 
* with the increasement of trip durations, number of riders tends to decrease.
* whether a user is a customer or a subscriber does have the biggest influence on results. Also age is an important factor, compared to gender which bairly affects any other variables in the data. 
