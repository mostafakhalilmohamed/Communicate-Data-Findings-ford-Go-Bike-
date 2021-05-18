# (Ford GoBike System Data)
## by (Mostafa Khalil Mohamed)


## Dataset
>This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco
Bay area.


> The dataset used for this exploratory analysis consists of monthly individual trip data from 1 febraury 2019 to 28 february 2019 in CSV format covering the greater San Francisco Bay area, also this dataset befor cleaning has 183412 rows and  16 coloumns such as (duration_sec,start_station_id,end_station_station_id,start_time,end_time,member_birth_year,member_gender,....)


> the main feature of interest in this dataset is duration_sec, i wiil use this column to get information and relation with another columns.


> Data wrangling process:
- convert stat_time column from object to datetime
- convert end_time column from object to datetime
- remove nan value from member_gender , member_birth_year columns, start_station_id,start_station_name,end_station_id,end_station_name
- Calculate member_age from member_birth_year
- change type of bike_share_for_all_trip from object to bool type



## Summary of Findings

> Trip Duration is so dependendable on the age of the member, when the age between 20 to 45, the trip duration is higher than the older ages. For the age, duration, and gender, for the others leap at an older age (around 60 years) to got 3000 trip duration. For the age, duration, and user type, both Customer and Subscriber are showing similar trends for age and trip duration, but for subscribers the trip duration is higher for older age.

## Key Insights for Presentation

> Distribution of Trip Durations: Trip Durations in the dataset take on a very large range of values. Number of Trips values first increases starting from around 8000 values to 12500 values at peak around 600 seconds but then starts to fall below at 2000 values.

> Distribution of User Age: In the case of age, the distribution is more concentrated between 20 to 40 years old.