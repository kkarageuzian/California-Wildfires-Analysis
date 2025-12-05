To create my visualization for my California Wildfire Analysis, I used a k-means clustering on wildfire latitude, longitude, and assessed property values 
(Assessed Improved Value (parcel)). The fires are separated into three geographic regions across California. The Southern and Central California region  
cluster is colored in red and located in the lower part of the state, the Northern Interior region cluster is colored in green and located in the central 
and upper inland area, and the Northern Coastal and Foothill Region is colored in blue and located along the coast. The clusters are formed based on the shape 
of California where the wildfires incidents tend to occur. There are also a few blue points that appear farther south, which is normal because k-means clustering 
groups fires based on all variables, so some individual fires match the coastal cluster even if they occur geographically lower on the map.

By looking at the point sizes, which represent the Assessed Improved Value (the dollar value of structures that were damaged), we can see that the Southern and 
Central regions experience most of the larger-loss events. This alludes to the fact that wildfires in this part of California tends to affect high-value 
properties/cause more severe damage. The Northern Interior region shows moderate losses, while the coastal and foothill region has smaller, less frequent high-value 
losses. Overall, the visualization helps highlight how wildfire impact varies by location and shows that the southern part of the state faces the greatest financial 
risk.


### California Wildfires: Clustering & Financial Impact Analysis

## Motivation
For this project, I wanted to explore how California wildfires vary across different regions of the state and whether certain areas experience more severe financial losses than others. Wildfires have become increasingly destructive in recent years, and I was interested in understanding the geographic distribution of high-damage incidents. This led me to ask, are there natural clusters in where wildfires occur, and which regions of California face the greatest financial risk?

## Data Source
The data for this project comes from the CAL FIRE Post-Fire Master Dataset, which records detailed information about wildfire incidents across California. This dataset includes key variables such as location (latitude and longitude), structure category, damage level, and Assessed Improved Value (parcel), which estimates the dollar value of damaged structures. The dataset was originally downloaded from the CAL FIRE database and then imported into R for cleaning and analysis.

## Processing Steps
To prepare the dataset for clustering and visualization, I performed several cleaning and transformation steps in Excel and R. 
