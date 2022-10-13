# Ford GoBike Exploratory Data Analysis
## by (Solomon 'Juwonlo Olorunleke)

## Dataset

> This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. Bay Area Bike Share is a company that provides on-demand bike rentals for customers in San Francisco, Redwood City, Palo Alto, Mountain View, and San Jose. Users can unlock bikes from a variety of stations throughout each city, and return them to any station within the same city. Users pay for the service either through a yearly subscription or by purchasing 3-day or 24-hour passes. Users can make an unlimited number of trips, with trips under thirty minutes in length having no additional charge; longer trips will incur overtime fees.
The source data (Ford GoBike System Data) is available at : https://s3.amazonaws.com/baywheels-data/index.html.

> My data consist of the information of the bike rides for the first four months of 2019. Some of the features in the dataset include:

- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
- Trip Duration(in seconds)
- Bike ID
- Start Time and Date
- End Time and Date
- Start Station ID
- End Station ID
- Start Station Name
- End Station Name
- End Station Latitude
- End Station Longitude
- Start Station Latitude
- Start Station Longitude

> For the wrangling, after downloading the data for each month individually, I combined them together in a compressed zip file and uploaded it into my working directory. I used Zipfile library to read the 4 csv files. For reading the data, I first used glob to find all the CSV files in my directory before using a for loop to read all 4 files at a go. I combined the datasets into into one and named it Ford2019.csv.

> I assessed the data programmatically, by looking into its head, tail, unique values, and value counts. I used info, describe, isnull and duplicated option to look deeper into the data 

> For the cleaning, I dropped the null values, dropped an irrevelant column, created more features that would aid my analysis and chnaged the features to the appropriate datatypes.

## Summary of Findings

>  The average duration for all trips is under 11 minutes.

>  Most trips were taken on Thursdays.

>  March recorded the highest number of trips.

>  The average distance travelled is about 2 kilometres.

>  The rush hours; going to work in the morning (8 and 9 hrs) and closing in the evening (17 and 18 hrs) have the highest trip records.

>  About 86.7% of the trips were taken by subscribers, with the remaining 13.3% coming from the customers.

>  Customers spend more duration than subscribers.

>  Trip durations on weekends are longer than on other weekdays.

>  Customer type doesn't really affect the number of trips per weekday.



## Key Insights for Presentation
> The average trip takes about 3 - 11 minutes and it is under 2 kilometres

> Thursday is the most popular day to use the Ford Go Bike sharing system in the Bay Area with over 150,000 rides. March records the most number of trips with over 250,000 trips also. 

> With the data queried for duration that are 30 minutes and under, customers normally have longer trip durations than subscribers. Customers normally ride between 8 minutes and 18 minutes. Subscriber trips are normally shorter and last anywhere between 5-13 minutes. 

> When viewed by month and without setting limits,  customers had similar trip durations with subscribers for February to April. The trip duration for customers in January are slightly higher than subscribers'.

> The average trip duration has been fluctuating by the month. There was a decrease from January to February, a very significant increase for March and a decline again in April. This goes to show that there is no definite relationship between the two variables.