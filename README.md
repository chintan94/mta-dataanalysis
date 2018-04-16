# mta-dataanalysis

This project was learning task in wrangling with data of turnsite provided publicly by MTA. (Can be found here http://web.mta.info/developers/turnstile.html)
- - - -
The Util method old_format_to_new clears the MTA formate of 8 Entry Exit data in one row to 1 entry exit data per row. 

The ca_station.csv maps a C/A to a station. The following is an example.

`df2['station'] = df2['C/A'].apply(lambda x: ca_station_map[x] if x in ca_station_map.index else 'UNDEF' + x`

Both the problems were resolved after 10/18/14. So for later files the processing is faster because no pre-processing is required.
- - - -
I solved the following problems for practice. 

## Data analysis
1) Which station has the most number of units as of today?
2) What is the total number of entries & exits across the subway system for August 1, 2013?
3) Let’s define the busy-ness as sum of entry & exit count. What station was the busiest on August 1, 2013? What turnstile was the busiest on that date?
4) What stations have seen the most usage growth/decline in 2013?
5) What dates in 2013 are the least busy? Could you identify days in 2013 on which stations were not operating at full capacity or closed entirely?

## Visualization
1) Plot the daily row counts for data files in Q3 2013.
2) Plot the daily total number of entries & exits across the system for Q3 2013.
3) Plot the mean and standard deviation of the daily total number of entries & exits for each month in Q3 2013 for station 34 ST-PENN STA.
4) Plot 25/50/75 percentile of the daily total number of entries & exits for each month in Q3 2013 for station 34 ST-PENN STA.
5) Plot the daily number of closed stations and number of stations that were not operating at full capacity in Q3 2013.

- - - -
More ideas on what can be done with it are welcomed. Would love to implement any learning task or correlation taks.
