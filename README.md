# Data Analysis - California Collision History 2001-2020

## Motivation 
According to the [CDC](https://www.cdc.gov/injury/features/global-road-safety/index.html), road crashes are a leading cause of death in the United States for people aged 1-54. It is estimated that fatal and nonfatal crash injuries will cost the world economy approximately $1.8 trillion dollars from 2015-2030(.12% of global GDP). 

Having lived in California since the early 80s, I was curious to analyze the historical automobile collision trends in California. This data will be valuable to federal, state and local governments to create plan public policy and local/state laws around driving. Information from the dataset can also be used to traffic police. These methods can be helpful in reducing the $1.8 trillion dollar cost of fatal and nonfatal crash injuries.

## Data

* This dataset comes from the California Highway Patrol [CHP Data Set](https://www.kaggle.com/alexgude/california-traffic-collision-data-from-switrs). It covers collisions from Jan 1,2001 to October 2020.  The dataset was consolidated by fellow data scientist Alex Gude. 
* There are 3 main tables. The collisions table has 74 columns, parties table has 31 columns and victims table has 11 columns.

    1. collisions: Contains ~9.17 Million rows.Contains information about the collision, where it happened, what vehicles were involved. 9.17 Million rows
    2. parties: Contains ~18Million rows. Contains information about the groups people involved in the collision including age, sex, and sobriety.
    3. victims: Contains ~9.17 Million rows. Has information about the injuries of specific people involved in the collision.

## Exploratory Data Analysis

* Several of the 74 columns contained data that was not useful to my analysis. For example, police officer codes
* My analysis of the 20 year automobile collision trends led me to use a few columns heavily: killed_victims, cellphone_use, latitude, longitude, male/female, alcohol_involved

