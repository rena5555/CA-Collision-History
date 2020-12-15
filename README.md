# Data Analysis - California Collision History 2001-2020

## Motivation 
According to the [CDC](https://www.cdc.gov/injury/features/global-road-safety/index.html), road crashes are a leading cause of death in the United States for people aged 1-54. It is estimated that fatal and nonfatal crash injuries will cost the world economy approximately $1.8 trillion dollars from 2015-2030(.12% of global GDP). 

Having lived in California since the early 80s, I was curious to analyze the historical automobile collision trends in California. This data will be valuable to federal, state and local governments to plan public policy and create local/state laws around driving. Information from the dataset can also be used to police traffic. These methods can be helpful in reducing the $1.8 trillion dollar cost of fatal and nonfatal crash injuries.

## Exploratory Data Analysis

* This dataset comes from the California Highway Patrol [CHP Data Set](https://www.kaggle.com/alexgude/california-traffic-collision-data-from-switrs). It covers collisions from Jan 1,2001 to October 2020.  

* There are 3 main tables. The collisions table has 74 columns, parties table has 31 columns and victims table has 11 columns.

    1. collisions: Contains ~9.17 Million rows.Contains information about the collision, where it happened, what vehicles were involved. 9.17 Million rows
    2. parties: Contains ~18Million rows. Contains information about the groups people involved in the collision including age, sex, and sobriety.
    3. victims: Contains ~9.17 Million rows. Has information about the injuries of specific people involved in the collision.

## Exploratory Data Analysis

* My analysis led me to use a few columns heavily: killed_victims, cellphone_use, latitude, longitude, male/female, alcohol_involved

* Using the latitude and longitude columns, I produced a heatmap to visually look at where the majority of the collisions occurred in the last 20 years. Out of 9.17 million rows, only 2.52 million had data. 


    ![picture](images/heat_map_2.png)

    * San Francisco county is the highest in density in the state of California. Orange and Los Angeles follow as second and third. It makes sense that the highest density locations is where the heat map is most red, representing higher number of collisions.

* 86% of the total collisions in the dataset are automobile accidents. The rest of the collisions are
bicycle, motorcycle, pedestrian, and truck collisions.

* Here is a closer look at the automobile collision history. Having normalized for population, the below graph shows the crashes per 1000 people over the course of 20 years.

    ![picture](images/collision_history.png)

    * Crashes were in the 12-14 crashes per 1000 people range from 2001 to 2007. In 2008, the crashes steadily dropped for several years until 2013 when they started going back up, but never as high as the initial trend. In 2020, the crashes dropped by almost 50% due to COVID 19.

## Statistical Test

* I was curious to map the unemployment rate % to see how well it correlated with crashes. This graph is exaggerated due to the different y axes. We can see from 2001-2006 there was a slight positive correlation between crash rates and unemployment rate. From 2008 to 2020, there seems to be an inverse correlation.

    ![picture](images/collision_unemp.png)
    
* The Pearson R correlation is -0.57. There is a moderately inverse correlation between unemployment rate % and crashes per 1000 people. This makes sense because crashes will drop when less people are driving to work.

* The unemployment rate went up from 2007 to 2010 due to the Great Recession. It was the worst and longest standing financial crisis in the United States since the 1929 Depression. Subprime mortgage was the trigger. 

* In July 2008, [California State Bill 28](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4001674/ ) went into effect. It banned the use of cell phones for texting while driving a motor vehicle.

* In future research, I would explore these factors that may correlate somewhat to a drop in collisions
    1. Stricter California vehicle stafety standards
    2. Smarter cars - sensors, AEB(automatic emergency braking)
    3. Driver distratcion related accidents(such as weather)
    4. Increase in carpooling or using buses and trains

            
            

        