# PyBer_Analysis

Module: Module 5
Student: Soona Britney Cheon
Date: October 25, 2020

1. Overview of the Analysis

The pursose of this project is merging 2 excel data (city_data, csv, ride_data.csv), analize the insightful data of each city type (urban, suburban and rural) to create the below:
1) A ride sharing sumamry Dataframe by city type including total rides, total drivers, total fares, average fare per ride, average fare per driver
2) A multiple-line chart of total fares for each city type to demonstrate the trend of the weekly total fare 


Results

1) A ride sharing sumamry Dataframe by city type
     a)The city_data consists each 120 city's drivers count, and the city type(Urba, Suburban, Rural), while ride_data consists 2,375 individual ride data including city, date, fare, and ride_id. By combining the 2 data files, we could have a better understanding about each ride, including city, city type, date, and fare.
     b) we could generate, 
        - total rides for each city type 
        - total drivers for each city type
        - total amount of fares for each city type
        - average fare per ride for each city type
        - average fare per driver for each city type
     c) findings
         - Urban city type has the highest number of rides (1,625), the highest number of drivers (2,405), and the highest sum of fares ($39,854.38).it is much longer in rural coty
         - Rural city type has the lowest number of rides (125), the lowest number of drivers (78), and the lowest sum of fares ($4,327.93)
         - Suburban city type has the middle range number of the rides (625), drivers (420), and the sum of fares ($19,356.33).
         - Although, for the average fare per ride, rural city type showed the highest ($34.62), shburban city type showed the next ($30.97), and the urban showed the lowest ($24.53). It means the average ride in urban city type is mush shorter, while the average ride in rural is much longer. 
         - For average fare per driver, the drivers in rural was the highest ($55.49), suburban ($39.50) was the next, and the urban ($16,57) was the lowest. it means, in urban, the average ride is short (=lower fare) and there are too many drives, so the income for each driver is lowest.   


2) A multiple-line chart of total fares for each city type
    a) Goal of the multiple-line chart - we wanted to illustrate the comparison of weekly total fare in each city type. 
    b) technics 
        - we calculated the total fare from the merged dataset
        - grouped by date and city type (urban, suburban, rural)
        - we reset the index as date by utilizing the pivot function.
        - once we have the daily date, we organzied as datetime format 
        - resampled as 'Week' function to prepare the multiple line graph 

    c) Conclusion - the weekly sum of the fare per city type showed the below:
        - Urban city type showed the hghest total weekly fare for 19 weeks
        - Suburban city type showed the middle 
        - Rural city type showed the lowest total weekly fare

Summary

The finding in each city type is as below:
1) Total Number of Rides: Urban (1,625) > Suburban (625) > Rural(125)   
2) Total Drivers: Urban (2,405) > Suburban (490) > Rural(78) 
3) Total Fares: Urban ($39,854.38) > Suburban ($19,356.33) > Rural($4,327.93) 
4) Average Fare Per Ride: Urban ($24.53) > Suburban ($30.97) > Rural($34.62) 
5) Average Fare Per Driver: Urban ($16.57) > Suburban ($39.50) > Rural($55.49) 

We found the total number of rides, total number drivers, and the total fare are greatest in urban city type.
Although, the average fare per ride is highest in rural city type.
Thus, the drivers in rural city type make more fare per driver. 

Thank you! 
