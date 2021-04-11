# Citibike Analysis using Tableau
## Overview of the Analysis
This analysis uses data from Citibike's public API describing user rides in August of 2019. The purpose of this analysis is to derive high-level insights from data visualizations, with a particular focus on peak use hours and differences in user patterns by gender.  

![https://public.tableau.com/profile/frank.feder#!/vizhome/Challenge14FrankFeder/CitibikeAugust2019?publish=yes](All visualizations can be viewed interactively at the Tableau Story here.)

## Results: All Users 
**Peak Hours**
The peak hours for August align with "rush hour" commuting periods. 8-9am and 4-7pm are the most popular times for customers to use the bikesharing service.

**Peak Days**
There are slightly more uses of the bikesharing service on Thursday, Friday, and Saturday - the last is interesting considering the previous graph, as on the weekend there are much less people commuting to work during rush hour periods. 

**Checkout Duration**
A majority of the rides in August 2019 were shorter than 30 minutes. A small amount of rides last much longer.

## Results: By Gender
**Rides by User Gender**
A large majority of rides in August 2019 were by users who specified the gender MALE. About 25% of all rides were by users who specified the gender FEMALE. 72% of users that provided a gender specified MALE, and 28% of users that provided a gender specified FEMALE. That's about 2.5x as many MALE users than FEMALE users.

**Checkout Duration by Gender**
The checkout duration is fairly consistent across all genders - a majority of rides by all genders are less than 30 minutes. The most common trip duration for MALE users is about 5 minutes, and for FEMALE users the most common trip duration is 6 minutes. 

**Peak Days by Gender**
Non-subscriber users used the bikesharing service most frequently on Saturday and Sunday, whereas Subscriber users more consistently used the service during weekdays. As expected per the "Riders by User Gender" graph, there are many more MALE rides described here than FEMALE or UNKNOWN. There is a consistent drop in service use on Wednesday, however - the cause could be interesting to investigate.

**Trips by Weekday by Gender**
For MALE and FEMALE users, rush hour commuting times were the most frequent in the measured period - considering the skew in user gender demographics, FEMALE users are fairly similar to MALE users in the concentration of service use around commuting hours. The weekends are a different story - while both MALE and FEMALE users are more likely to use the service in the early afternoon hours on the weekends, the amount of trips by FEMALE users during this time actually outweighs MALE user trips during these times, after adjusting for Citibike's gender demographic skew. For example, if we look at 2pm on Sundays in the measured period, there were ~6k rides by FEMALE users and ~12.5k rides for MALE users. To adjust for demographic skew we can multiply the FEMALE rides by 2.5x, so the adjusted count is ~15.3k FEMALE to ~12.5k MALE. Judging by this disparity, **FEMALE users are 22% more likely to use the service during Sunday afternoons than MALE users.**



## Summary
In conclusion, the Citibike service had the most utilization during popular commuting hours during August 2019. The majority of those rides were under 20 minutes, with very little difference in ride duration trends between user gender groups. A huge majority of the service's users during this time were MALE, and only 25% of rides during this period were by FEMALE users. Thursdays, Fridays, and Saturdays were the most popular days for Citibike use, and the least rides occured on Sundays and Wednesdays. There is a slight difference in user behavior when grouped by gender, with MALE users more likely to use the service during commuting hours and FEMALE users more likely to use the service during weekend afternoons.

### Additional Visualizations
In future analyses, the following visualizations may provide worthwhile insights:
1. Average Service Revenue per Ride, by Weekday 
2. Service Revenue by Gender, by Weekday
3. Long-Duration Ride Location Map