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

These visualizations are interactable and are available to view on [Tableau Public](https://public.tableau.com/views/CitiBike_Aug2019_NYC_FullStory/NYCCitiBikeAug2019?:language=en-US&:display_count=n&:origin=viz_share_link) as well. 

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

Subscribers and male riders are the primary demographic that contributes the most to the count of trips. Majority of the subscribers exhibit a consistent trip duration of 5 mins whereas customers tend to have longer trips that are more evenly distrubted across 10 - 26 minutes. The subscriber trip duration trend is observed proportionally between the male and female demographics but the unknown demographic loosely follows the trend for customers with longer trip durations distributed evenly. The disparity between the unknown demographic and the customer demographic can be accounted for in the trend for female and male riders as there are minor bumps in the trend as the peaks taper off. Peak riding hours coincide with morning and evening commute times and there are more rides during daylight hours. This can be assessed clearly in the following heatmap that displays higher trip counts during the weekday commuting hours from Monday to Friday but a more dispersed model across daylight hours closer to the weekend. This trend is maintained across the gender and clientle demographics with male riders and subscribers contributing the most to trip counts. It is important to note the similar but faint signature for the unknown and customer demographics that show more activity during daylight hours of the weekend. The final heatmap recapitulates all the aforementioned trends and most notably the fact that most of the subscribers have declared genders and that the majority of customers are unknown gendered. *Note: Some visuals below require visiting Tableau Public to fully visualize the data.* 

  - ![Checkout Times for Users](https://github.com/Fabalin/bikesharing/blob/main/Tripsbyclientele.PNG)
  - ![Checkout Times by Gender](https://github.com/Fabalin/bikesharing/blob/main/tripsbygender.PNG)
  - ![Peak Riding Hours](https://github.com/Fabalin/bikesharing/blob/main/peakcommute.PNG)
  - ![Trips by Weekday for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsbyweek.PNG) 
  - ![Trips by Gender for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsweekgender.PNG)
  - ![Trips by Clientle for Each Hour](https://github.com/Fabalin/bikesharing/blob/main/tripsandclientle.PNG)
  - ![User Trips by Gender by Weekday](https://github.com/Fabalin/bikesharing/blob/main/weeklytripsgenderclientele.PNG)

**Characterizing Bike Usage Geographically across Demographic Groups.**

Bike usage purpose can be intiuited from geographical data. The scatter plots demonstrate that the distribution of trip density in Manhattan and the largest density can be observed spread across the commerical districts of Central Manhattan that experience high population density due to commerical activity. These visuals are interactive on [Tableau Public](https://public.tableau.com/views/CitiBike_Aug2019_NYC_FullStory/NYCCitiBikeAug2019?:language=en-US&:display_count=n&:origin=viz_share_link). Although not filtered below, the male and subscriber populations contribute the most to the density of the first visual. When filtering for customers only, the distribution shifts dramatically to be more localized near scenic areas. These include waterfront areas and the periphery of the Central Park. ALthough not filtered below, the male and female populations still maintain this trend but the unknown gendered riders contribute the most to the density observed.  

  - ![Top Starting Locations All](https://github.com/Fabalin/bikesharing/blob/main/commutetowork.PNG)
  - ![Top Starting Locations Customers](https://github.com/Fabalin/bikesharing/blob/main/sceneic.PNG)

**Characterizing Bike Usage with Total Trips and Duration.**

In order to assess the longevity of the bikes in deployment and to gauge potential maintanance costs, the frequency and duration of bike usage is visualized below. The first visual is a clustered tree map that displays groups of bikes that fall within a certain trip frequency. Majority of the bikes (estimated visually to be greater than 50%) have been through 90 - 222 trips and they are denoted by the pink and teal blue clusters. Within the remaining clusters, the red cluster bikes experience one of the highest total trips with the minimum being 307 trips and the maximum being 479 trips. Second to this, there are a few bikes whose trip totals range between 223 - 306 trips. Although hard to visualize due to scale, there are even more bikes that have smaller trip totals of between 1 - 89 trips. The following circle plot conveys the total trip duration of individual bikes. An overwhelming majority of bikes have duration totals of around 3 - 4 days. The remaining visibly large circles convey bikes that have up to 10 days and the countable, darker circles have a maximal duration of over a month.    

  - ![Bike Usage based on Trips](https://github.com/Fabalin/bikesharing/blob/main/majorityusage.PNG)
  - ![Bike Usage Duration](https://github.com/Fabalin/bikesharing/blob/main/tripduration.PNG)

## Summary 
Citi Bike works in New York due to its setting. Manhattan is a small, densely populated urban sprawl that features one of the world's largest commerical hubs. Public transportation is crucial in these settings and even more so, a cost efficient, space saving model is preferred. From the results presented, it is evident that people use Citi Bikes to commute to and from work during the weekdays and to explore the city during the weekend. The high male rider population can be explained in multiple ways but the best approach is to understand the inherent factors associated with bike commutes as it requires physical exertion and the safety of the rider is dpenendent on the neighborhood of commute. More subscribers use the bikes than regualr customers suggesting that the business model and setting facilitate brand loyalty, either through cost and/or utility. Customers are less likely to declare their gender and Subscribers are more likely to declare their gender as user information provided scales with investment towards the service. There is a distinct shfit in the relevant usage purpose betweem subscribers and customers. Based on the trip duration by Usertype and the scatterplot of trip density, Subscribers tend to use the bikes for short commutes to-and-from work whereas Customers primairly use the bikes for leisure and recreational purposes. Although additional data is required to fully estimate the projected spend on maintanance for bikes there are two metrics by which the possible spend on repairs can be gauged. Bikes with the total number of trips that fall into the orange or red culsters should be accounted for as higher total trip numbers are likely to correlated with more wear and tear. This is also true for bikes with higher trip durations. Following this model, there are fewer bikes that will require maintanance than bikes that are in circulation. 
