# Bay Wheels' Trip Data Exploration and Visualization


## Dataset (Ford GoBike)

This document explores a dataset containing [information](https://www.lyft.com/bikes/bay-wheels/system-data) about individual rides made in [Bay Wheels](https://en.wikipedia.org/wiki/Bay_Wheels)' bike-sharing system covering the greater San Francisco Bay area.  The dataset is data from January 2019 and can be manually downloaded [here](https://s3.amazonaws.com/baywheels-data/index.html).

## Summary of Findings

Trip durations in the dataset take on a very large range of values, from about 1 minute at the lowest, to about 23.3 hours at the highest.  Thursdays are the busiest with the highest trip count.  There are more trips during the weekdays than there are during the weekends.  The likely reason for this may be due to the service being used for work commutes.  This claim can be backed up by the plot showing that trip counts peak at 8 AM and 5 PM (those would be the normal working hours).

There are two types of users using this bike sharing service, Subscribers and Customers.  There are more Subscribers taking trips than Customers.  

On Sundays and Saturdays, trips counts are the highest between 2-3 PM.  Mondays through Fridays, trip counts peak at 8 AM and at 5 PM.  Looking at this through the lens of user type, Customers trip counts peak at 8 AM and 5 PM.  That is the same for Subscribers, but the difference is that there are more Subscribers than Customers.  

Subscribers use the service the most on Thursdays, while Customers use the service the most on Saturdays.  Subscribers have much shorter trips than Customers on a daily basis, but both of them do have an increased trip duration on weekends.  

## Key Insights for Presentation

- Subscribers use the service heavily Mondays through Fridays, while Customers ride a lot on weekends.
- Subscribers usage concentrated around work hours, which is around 8 AM and 5 PM.  Customers tend to use the service more aroudn 2 PM.
- Subscribers have shorter trips than Customers.

## Sources

- https://en.wikipedia.org/wiki/Bay_Wheels
- https://www.lyft.com/bikes/bay-wheels/system-data
- https://s3.amazonaws.com/baywheels-data/index.html
- https://stackoverflow.com/questions/20906474/import-multiple-csv-files-into-pandas-and-concatenate-into-one-dataframe
- https://stackoverflow.com/questions/25129144/pandas-return-hour-from-datetime-column-directly
- https://pythontic.com/datetime/date/weekday
- https://stackoverflow.com/questions/9847213/how-do-i-get-the-day-of-week-given-a-date
- https://stackoverflow.com/questions/53398259/create-histograms-for-all-categorical-variable-values
- https://stackoverflow.com/questions/17109608/change-figure-size-and-figure-format-in-matplotlib/17109830
- https://datavizpyr.com/countplot-or-barplot-with-seaborn-catplot/
- https://seaborn.pydata.org/generated/seaborn.heatmap.html