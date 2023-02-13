# Google Data Analytics Capstone Project using Divvy bike data

*View the R Script:* **[HERE](https://github.com/jamiedeocampo/bike-share-analysis/blob/main/bike-share-analysis.R)**<br />

This Case Study was completed as part of the Google Data Analytics Professional Certificate.

1. Objective (Ask Phase)

To analyse how annual members and casual riders use bikes differently in order to determine the best marketing strategy to convert casual riders into annual members.

2. Prepare Phase

The data was downloaded directly from the Divvy Bikes website: https://www.divvybikes.com/system-data

3. Process Phase

After regularising and importing the data, the first step was to inspect each attribute for anomalies.  

There are a few problems we will need to fix:
1. In the "member_casual" column, there are two names for members ("member" and "Subscriber") and two names for casual riders ("Customer" and "casual"). We will need to consolidate that from four to two labels.
2. The data can only be aggregated at the ride-level, which is too granular. We will want to add some additional columns of data -- such as day, month, year -- that provide additional opportunities to aggregate the data.
3. We will want to add a calculated field for length of ride since the 2020Q1 data did not have the "tripduration" column. We will add "ride_length" to the entire dataframe for consistency.
4. There are some rides where tripduration shows up as negative, including several hundred rides where Divvy took bikes out of circulation for Quality Control reasons. We will want to delete these rides.

4. Analyse Phase

In this phase, queries were created to uncover trends that were highlighted in the data visualisations.

5. Share Phase

Visualisations were created using Tableau.

6. Act Phase

A powerpoint presentation was compiled - Cyclistic - Annual Members differ Casual Riders.pptx.

### Raw CSV Files
![img-q2_2019-raw](visuals/img-q2_2019-raw.png)
![img-q3_2019-raw](visuals/img-q3_2019-raw.png)
![img-q4_2019-raw](visuals/img-q4_2019-raw.png)
![img-q1_2020-raw](visuals/img-q1_2020-raw.png)

### Combined and Cleaned
![img-all-trips-cleaned-01](visuals/img-all-trips-cleaned-01.png)
![img-all-trips-cleaned-02](visuals/img-all-trips-cleaned-02.png)

### Visualization for number of rides by rider type
![Visualization for number of rides by rider type](visuals/img-visual-rides-by-rider.PNG)
### Visualization for average duration
![Visualization for average duration](visuals/img-visual-average-duration.PNG)
