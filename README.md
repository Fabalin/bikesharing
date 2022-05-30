# Bikesharing
Using Tableau to create data visualizations. 

## Overview 
Citi Bike is a bikesharing program that is popular in NYC due to its feasibility and utility in an urban setting. In order to assess the viability of the business model, ride data from August 2019 was visualized using Tableau across multiple metrics. The original data file was sourced directly from [Citi Bike](https://ride.citibikenyc.com/system-data) as a CSV file. The file was then processed using JupyterNotebook to convert tripduration column into a datetime format. The resulting file was used to create visualizations below in order to determine its feasibility in the city of Des Moines: 

- Total Trips 
- Clientle 
- Gender Breakdown
- Checkout Times for Users
- Checkout Times by Gender
- Trips by Weekday for Each Hour 
- Trips by Gender for Each Hour
- Trips by Clientle for Each Hour
- User Trips by Gender by Weekday
- Peak Riding Hours
- Top Starting Locations
- Bike Usage based on Trips 
- Bike Usage Duration

These visualizations are available to view on [Tableau Public](https://public.tableau.com/views/CitiBike_Aug2019_NYC_FullStory/NYCCitiBikeAug2019?:language=en-US&:display_count=n&:origin=viz_share_link) as well. 

## Software
- Tableau Public - 2022.1
- Jupyter Notebook - v 6.4.11

## Results
**Total Number of Trips and Demographic Assessment: Clientle and Gender Breakdown.**

Among the 2,344,224 recorded rides, 81% were Subscribers and 65% were male. Female riders make up a quater of the riders with less than 10% riders being gender unknown. Customers that are not subscribers make up 19% of the total trips. 

  - ![Total Trips](https://github.com/Fabalin/bikesharing/blob/main/total_trips.PNG)
  - ![Clientle](https://github.com/Fabalin/bikesharing/blob/main/Clientele.PNG)
  - ![Gender Breakdown](https://github.com/Fabalin/bikesharing/blob/main/Gender.PNG)

**Characterizing Bike Usage Temporally across Demographic Groups.**

  - ![Peak Riding Hours](https://github.com/Fabalin/bikesharing/blob/main/peakcommute.PNG)
  - ![Checkout Times for Users](https://github.com/Fabalin/bikesharing/blob/main/Tripsbyclientele.PNG)
  - ![Checkout Times by Gender](https://github.com/Fabalin/bikesharing/blob/main/tripsbygender.PNG)
  - ![Trips by Weekday for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsbyweek.PNG) 
  - ![Trips by Gender for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsweekgender.PNG)
  - ![Trips by Clientle for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsandclientle.PNG)
  - ![User Trips by Gender by Weekday](https://github.com/Fabalin/bikesharing/blob/main/weeklytripsgenderclientele.PNG)

**Characterizing Bike Usage Geographically across Demographic Groups.**

  - ![Top Starting Locations All](https://github.com/Fabalin/bikesharing/blob/main/commutetowork.PNG)
  - ![Top Starting Locations Customers](https://github.com/Fabalin/bikesharing/blob/main/sceneic.PNG)

**Characterizing Bike Usage Frequency and Duration.**

  - ![Bike Usage based on Trips](https://github.com/Fabalin/bikesharing/blob/main/majorityusage.PNG)
  - ![Bike Usage Duration](https://github.com/Fabalin/bikesharing/blob/main/tripduration.PNG)

## Summary 
