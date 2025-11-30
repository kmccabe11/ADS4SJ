# ADS4SJ
# Exploring CAHOOTS' Response Time in Eugene

### Background 

As of April 7th, 2025, due to funding and resources CAHOOTS (Crisis Assistance Helping Out On The Streets) is no longer operating in Eugene. CAHOOTS has built a reputable name and a great sense of trust within the Eugene and Springfield areas, however this cannot be measured and therefore has limitations on its ability to be used to advocate for CAHOOTS. As CAHOOTS is currently advocating to obtain funding and operation, it is important to address the critiques that CAHOOTS has received. I will be focusing on addressing the concern of CAHOOTS’ response time in Eugene. This is in reaction to the criticism that it takes CAHOOTS more time than it should to get to a dispatched call, which decreases their value and effectiveness. 

I will investigate this concern by looking into response time, how it has varied over time, and what factors might impact it. Understanding these things will not only provide an informed view of CAHOOTS’ response to a call, but it could aid CAHOOTS in improving their efficiency. 

### Data:

The data that I used is computer-aided dispatch data in Eugene from 2014 - April 2025. Each individual year is its own dataset containing each dispatched call in Eugene for that year.  The strengths of this data are how in-depth it is, containing every dispatched call spanning 11 years, however a limitation is that there is not a great amount of description of the data. Therefore, some of the variables don't have documentation on how they were calculated or collected. Additionally, there is no note of any data entry error that may be present. 

Raw dats is contained in the CAD_data_through_2025 folder

### Data Cleaning:

To clean the raw data download CAD_clean.ipynb

Cleaned Data:
- call.csv
- cahoot.csv

### Data Analysis

Download and run CAD_analysis.ipynb

Packges you will need: 
- Pandas
- Numpy
- Matplotlib.pyplot
- Seaborn
- Datetime
- Scipy.stats

### Discussion

This analysis set out to investigate the criticism and concern that CAHOOTS’ response time is too slow, which can take away from their value and impact. Looking into response time and call volume, my results show that while call volume does play a role in CAHOOTS’ response time, it is not the sole or primary driver of these changes in efficiency. Since 2014, response times have clearly improved, even when call volume fluctuation would not suggest improvements. This points towards additional factors influencing response time, or operational improvements within CAHOOTS. 
I next looked into additional factors such as call priority, month, daily call density, and call nature to better understand the shifts in response time. While I expected there may be an effect of seasonal change or the University of Oregon schedule on response time, I found that CAHOOTS had a very consistent response time throughout the year. CAHOOTS also performs well on high-volume days, showing that they are able work efficiently even on their most demanding days. Call nature was one of the few factors that indicated an inconsistent response time across its variation. Even when avoiding outliers, average response time shifts across different call natures. This is what I would expect, and since “Found Contraband” had the slowest response time, this indicates a beneficial allocation of resources. If a “Suspect Down” call and a “Found Contraband” call are both dispatched to CAHOOTS, it is a good sign that the "Suspect Down” incident would take precedence, be responded to first, and therefore have a faster average response time. 
When looking into priority, it was evident very quickly that the great majority of CAHOOTS calls are priority 7 or 5. This leads me to ask questions on the process of dispatching a call to CAHOOTS. Is there a standard priority to use? Do the most common call natures CAHOOTS respond to coincidentally fall into priority 7? It is unclear whether the process of dispatching a CAHOOTS call involves labeling it with a specific priority in a consistent or meaningful way. Since priority distribution shifted significantly after 2022, especially with most CAHOOTS calls labeled as lower priorities in later years, I did not feel confident in understanding and concluding answers on how call priority affects CAHOOTS’ response time. 
What I did find valuable from the priority data was comparing EPD and CAHOOTS response time on individual priorities. The priorities that had the greatest amount of calls dispatched to CAHOOTS had the smallest gap between EPD and CAHOOTS response time. This was a surprising relationship I did not expect to find. I would be curious to look further into the presence of outlier response times in priorities with a low volume of calls dispatched to CAHOOTS, since these would be more influential to the overall response time comparison. 
Through time, the gap between EPD response time and CAHOOTS response time is narrowing. And while EPD consistently outperforms CAHOOTS in response time, it's important to note that my analysis doesn’t account for the substantial difference in staffing, capacity, and general resources, all things EPD takes the advantage on. It also does not consider EPD’s ability to travel faster than any vehicle on the road while using sirens and lights. In response to the concern that CAHOOTS is inefficient or slow, I think it is crucial to evaluate their operational limitations in comparison to EPD. 
Caveats to this analysis include extreme outliers, while initial testing excluding outliers showed the same or very similar results and trends, it could be a more robust approach to identify and address the extreme outliers in the data. There was no documentation of data entry errors, however CAHOOTS calls dropped to 0 through all of January of 2023. I did not find documentation of CAHOOTS not being in service during this time or another city wide reason, so I expect this was an error in the data. 
The year 2023 stands out as a major inflection point across many different pieces of the data: call volume declined, response time dropped, and large shifts were visible in priority of calls and call natures. To expand this analysis, I am most curious about possible causes to this since the decreased response time has remained consistent. Through my analysis, CAHOOTS has improved their efficiency in arrival time. There is a weak correlation between call volume and response time, so while lower call volume may be contributing, it is likely not the driving factor of the growth in efficiency. Determining additional influences to this improvement is still unanswered, whether it is due to specific qualities of the calls being assigned to CAHOOTS, a shift in Eugene’s needs, or a shift in how CAHOOTS is operating. In addition to investigating what would cause this change based on the year, I would be very interested to include the information of EPD’s resources, and compare the agencies based on their capacity. 

