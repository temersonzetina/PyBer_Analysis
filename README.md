# PyBer_Analysis

## Overview
The purpose of this analysis is to provide insights to executives at PyBer, a ride-sharing company, about the company's key results over the course of a 4-month span in 2019 by city type (urban, suburban, and rural). Equipped with the information provided herein, executives will be able to observe trends and disparities that can inform strategic priorities moving forward.

The steps involved in conducting this analysis are immediately below:

1. Clean and merge the key data sources, which include (1) a file with ride-level data and (2) a file with information about each city's driver counts (NOTE: The ride-level file captured information from January through April 2019, hence the findings below derive from data from that period alone)
2. Gather aggregate indicators by city type (Total Rides, Total Drivers, and Total Fares)
3. Use these aggregate indicators to calculate Average Fare/Ride and Average Fare/Driver
4. Visualize these data into a table
5. Calculate and store fare totals by date and city type
6. Visualize these totals in a line plot

## Results
The figure below illustrates the differences in key results by city type. The sub-sections that follow describe these differences in context.

![Ride data dataframe](https://github.com/temersonzetina/PyBer_Analysis/blob/main/PyBer_ride_data_by_city_type.png)

### Total Rides
Rural towns had fewer rides (125) than suburban (625) and urban (1625) locales. Larger populations seem to predict more usage in terms of ride-sharing services.

### Total Drivers
The differences in total drivers by city type were far greater than differences in total rides, both in absolute terms and proportionality. The number of rural rides was one-fifth that of suburban rides, which were around 40% of urban rides. But the number of rural drivers was around one-sixth the number of suburban drivers, which were just 20% of the total number of urban drivers. The differences in total rides and total drivers represent important considerations for managing supply given demand (see summary section below).

### Total Fares
The proportion of total fares in rural areas to total fares in suburban areas was similar (roughly one-fifth) to the proportion of total drivers between these two city types. By contrast, suburban total fares were nearly half that of total fares in urban areas, which is well over double the proportion between these two in terms of total drivers.

### Average Fare per Ride
Rural fares per ride were around 13% higher than suburban fares, which were around a quarter higher than urban rides. The ratio of drivers to total rides in rural areas - which is by far the lowest for all city types - likely explains why rural average fares per ride were highest. It may also be the case that rural areas, which are by nature more spread out than urban areas, have longer, more costly rides.

### Average Fare per Driver
Differences by city type in terms of average fare per driver were even greater than differences in Average Fare per Ride. Rural areas' average fare per driver was around 40% higher than that of suburban drivers. Suburban drivers, in turn, had an average fare that was approximately 1.5 times that of urban drivers.

### Total Fare by City Type (Chart)
The chart below demonstrates total fares for each week between the beginning of January and the end of April 2019. Each line plot represents one of the three city types.

![Fares_by_week](https://github.com/temersonzetina/PyBer_Analysis/blob/main/PyBer_fare_summary.png)

The plot trajectories share several similarities while also differing in multiple ways. Both urban and suburban areas began the calendar year on upward trends, whereas rural area performance was up and down. All three city types hit peaks in late February, and experienced varying levels of volatility in March. Rural and urban areas were on the decline towards the end of the period of study, while the suburbs began to gain steam.

## Summary
In light of the information presented above, below are three business considerations for addressing disparities and increasing revenue -

1. *Incentivize urban drivers to spend shifts in the suburbs.* Though it is difficult to conclude based solely off of these datasets, it may be the case that the surplus of urban drivers has a negative impact on average fare/ride. Given their relative proximity to suburbs, urban drivers may relieve some of this disparity by working in/around city limits and surrounding communities. Consider incentivizing urban drivers to spend shifts in suburban areas where there are relatively fewer drivers.
2. *Cap the number of urban drivers during certain hours to optimize supply given (anticipated) demand.* Building off of the assumption from #1 - that lower average fares/ride in urban areas may be due to driver surpluses - consider capping the number of urban drivers during certain times of the day. Establish a system, based on prior data about ride activity during certain times of day, in which the company optimizes the number of drivers on the road to address demand without creating surplus supply.
3. *Increase the number of rural drivers through a marketing campaign.* Again, it is difficult to make conclusions from this data alone about the relationship between drivers and rides. However, it is possible that in rural areas, part of what explains relatively low ridership is lack of supply. Consider increasing the number of rural drivers through a campaign that targets businesses and institutions in rural areas most likely to access ride-sharing services.
