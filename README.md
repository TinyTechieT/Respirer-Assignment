# Respirer-Assignment

## Problem Statement

The attached file contains data from a field experiment- energy meter readings (r1 to r12). The following are the column headers.

Time = timestamp at 1 hour granularity\
year = Year\
moy_date = Month of year\
doy_date = Day of year\
busday = Business day or Working day\
season = Season of the year\
dow_date = Day of week\
hour = Hour of the day\
temp = Temperature\
humid = Humidity


## Assumptions
* Meter readings are all of the same scale and there is no requirement for normalisation.

## Findings
Here are some of my findings in each of the 3 tasks. They are also present in the notebooks in between code cells.
### Task 1 - Data Visualization
* There weren't any null values.
* Most of the energy meters showed the highest energy meter readings in Summer as compared to the other seasons.
* More specifically, most of the energy meters showed the highest energy meter readings in May and June.
* Busy days and non-busy days did not have any effect on the energy meter readings.
* Most of the energy meters had lower readings during the day than in the night.

### Task 2 - ML
* The seasons, when plotted on the scatter plot, were not very distinctly clustered. But when split into busy and non-busy days, the clustering was much more distinct on non-busy days.
* Summer data points were spread all over the place.
* The K-Means algorithm was able to cluster one set of data points with moderate accuracy (I suspect that this was the monsoon cluster), one with low accuracy and the last one with poor accuracy.
* The K-Means algorithm resulted in a silhouette score of roughly 0.45, which indicated a moderate level of clustering.

### Task 3 - Statistics
* r12 had the highest mean and standard deviation of all the energy meters.
* r4 had the highest possible energy meter reading of all the meters.
* All the meters were skewed towards the right in the histogram analysis.
* The boxplots showed a lot of outliers, which could be due to measurement errors or unusual energy consumption.
* Most of the meters show a spike in the trend component around the summer months (March-June), which could mean increased energy consumption.
* Residuals have a large degree of randomness. But most of the meters show increases around the summer months which could mean increased energy consumption.
