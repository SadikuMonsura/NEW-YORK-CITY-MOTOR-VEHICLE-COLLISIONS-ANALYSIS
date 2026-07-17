# NEW-YORK-CITY-MOTOR-VEHICLE-COLLISIONS-ANALYSIS
An exploratory analysis of collision trends, contributing factors and safety 

![](Dashboard_Overview.png)

## EXECUTIVE SUMMARY

This report presents an exploratory analysis of motor vehicle collisions reported in New York City between 2021 and 2023. The objective was to identify collision trends across time, location and contributing factors while uncovering actionable insights that could support road safety initiatives and traffic management.

A total of 238,421 collisions were analyzed. These collisions resulted in 87,102 injuries and 613 fatalities, indicating that although most accidents were non-fatal, they still had a significant impact on public safety. 

The analysis found that collisions occurred most frequently during the afternoon rush hours, were highest on Fridays, and were predominantly caused by driver inattention/distraction and unspecified driver-related factors. Brooklyn recorded the highest number of collisions among all boroughs, while Belt Parkway emerged as the street with the highest collision frequency.

### Project Objectives 

The objectives of this analysis were to:

- Analyze monthly accident trends and identify seasonal patterns.
- Determine when accidents occur most frequently by day of the week and hour of the day.
- Identify the street with the highest number of reported collisions.
- Determine the most common contributing factors to collisions and fatal accidents.
- Generate additional insights that can support road safety improvements.

## DATASET DESCRIPTION

Each row in the dataset represents a single motor vehicle collision reported by the New York City Police Department.

The dataset contains the following information:

- Collision ID
- Date
- Time
- Borough
- Street Name
- Cross Street
- Latitude
- Longitude
- Vehicle Type
- Contributing Factor
- Persons Injured
- Persons Killed
- Pedestrians Injured/Killed
- Cyclists Injured/Killed
- Motorists Injured/Killed

### Data Preparation 

Before analysis, the dataset underwent several cleaning and transformation steps.

These included:

- Replacing missing values in the Borough column with "Unknown" to preserve all records.
- Creating Month, Weekday, and Time Period fields from the Date and Time columns.
- Grouping accident times into:
    - Morning
    - Afternoon
    - Evening
   - Midnight
- Validating numerical fields for injuries and fatalities.
- Removing unnecessary duplicates where applicable.
- Creating DAX measures for KPI calculations.

## METHODOLOGY

![](powerquery.png)

![](clean_dataset.png)

![](New_columns_and_metrics.png)

## ANALYSIS AND FINDINGS

### Key Performance Indicators (KPIs) 

| KPI     |    Value   |
| :--- | :---: |
| Total Collision | 238,421 |
| Accidents with Death | 613 |
| Accidents with injuries | 87,102 |
| Fatality Rate | 26% |
| Vehicle Types Identified | 17 |

The KPIs indicate that fatal crashes represent only a very small proportion of all reported collisions, while injuries occur in more than one-third of accidents. 

### Question 1: Percentage of Total Accidents by Month

The monthly analysis shows noticeable variations in accident frequency throughout the year.

Key observations include:
- March recorded the highest proportion of collisions at approximately 11%.
- January also recorded a high accident rate at approximately 10%.
- Accident frequency gradually declined after March.
- November and December recorded the lowest percentages, approximately 7%.

### Seasonal Pattern
The results indicate that accident frequency was highest during the first quarter of the year before gradually declining towards the end of the year. 

Possible contributing factors include:
- Increased traffic following holiday periods.
- Seasonal weather conditions.
- Changes in commuting patterns throughout the year.

### Question 2: Accident Frequency by Day of Week and Hour 

### By Day of Week:

Friday recorded the highest number of collisions with approximately 37,496 accidents, making it the most dangerous day of the week.

Possible reasons include:
- Increased commuter traffic.
- Weekend travel.
- Higher evening traffic volumes.

### By Hour of Day

Accidents were concentrated during the afternoon period.

The busiest accident period occurred between:

2:00 PM and 5:00 PM

This coincides with:
- School closing hours
- Evening rush-hour traffic
- Increased pedestrian activity

The fewest accidents occurred during the midnight period.

### Question 3: Street with the Highest Number of Collisions 

The analysis identified Belt Parkway as the street with the highest number of reported collisions.

Other high-risk streets include:
- Broadway
- Atlantic Avenue
- Long Island Expressway
- Brooklyn-Queens Expressway

Although Belt Parkway recorded the highest number of accidents, it represents only a small percentage (around 1.6%) of all reported collisions, indicating that collisions are widely distributed across the city's road network rather than concentrated on a single roadway.

### Question 4: Most Common Contributing Factors 

The leading contributing factor for reported collisions was:

Driver Inattention/Distraction

Other frequently reported contributing factors include:
- Unspecified
- Failure to Yield Right-of-Way
- Following Too Closely
- Passing or Lane Usage Improper
- Unsafe Speed
- Backing Unsafely

For fatal accidents specifically, driver-related behaviors such as distraction, unsafe driving practices, and failure to yield continued to be among the most significant contributing factors, highlighting the critical role of human behavior in severe crashes.





