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
