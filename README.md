# Tracking Critical COVID-19 Data

Johns Hopkins University recently released an updated component to their [Coronavirus Resource Center website](https://coronavirus.jhu.edu/data) that showcases both critical COVID-19 data trends and an in-depth look at the most up-to-date COVID-19 confirmed case and death reports by US county. These data visualizations can help us better understand the virus's spread across countries so that we can implement data-driven prospective measures, policies, and support to help minimize the spread of the virus and better understand who might be in need of supplies or other support while there are active cases in those US counties. 

Under Critical Trends, the [Cumulative Cases Over Time ](https://coronavirus.jhu.edu/data/animated-world-map)data visualization animation shows "the total number of cases reported in each country at each point in time, regardless of how many people have recovered:"

![](.gitbook/assets/jhu-covid19-global-animation.gif)

While this helps us understand the overall toll of the virus in a country at a given time, we've seen in the US how local state and city leadership is critical to  manage the well-being of their jurisdictions by protecting and informing citizens, forming public-private partnerships, and implementing social distancing and other policies to mitigate the spread of the virus and provide additional resources for healthcare frontline staff. An animated data visualization that demonstrates the number of cumulated COVID-19 confirmed cases in US counties can help us better understand how the virus is spreading within the United States and which county and state governments, businesses, and other organizations might need support during the pandemic.

 **How can we make a similar visualization to show the overall toll on US counties or county equivalents?**
 
 ## Business Question
 __How can we visualize and better understand the overall toll of the COVID-19 pandemic on US counties or county equivalents?__
 
 ## Data Question
__Which data and metrics can we use to answer our question?__
We'll use plotly express to build an animated [choropleth map](https://melanieshimano.gitbook.io/covid-19-critical-trend-data-visualizations/where-are-covid-19-cases-increasing-within-the-united-states) that shows the number of cumulative confirmed COVID-19 cases per 1,000 residents in US counties, but first, we'll review some geospatial data analysis in Python by making a bubble map and a density heat map to showcase the number of cumulative COVID-19 confirmed cases in each US county on today's date. 

We'll use data from the following sources for our analysis: 
 - [JHU CSSE COVID-19 Case Data](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports)
 - [New York Times COVID-19 Data](https://github.com/nytimes/covid-19-data/blob/master/us-counties.csv)
 - [US County Geospatial Data](https://raw.githubusercontent.com/plotly/datasets/master/geojson-counties-fips.json)
 
In our Python Notebooks we’ll use the following packages to conduct our analysis:
 ```
 pandas 1.0.3
 plotly 4.6.0
 urllib 1.25.8
 json 2.0.9
 ```
 
## Data Answer
The steps for our data analysis are available in [this GitBook tutorial](https://melanieshimano.gitbook.io/covid-19-critical-trend-data-visualizations/). You can use [this](https://github.com/jhu-business-analytics/covid-19-map-visualizations/blob/master/2020-04-14-covid19-cases-us-county-animation-gitbooktutorial-STARTER-melanieshimano.ipynb) pre-commented starter notebook to follow along with the tutorial, or copy and paste the code from the codeblocks (dark blue text boxes) in the tutorial.
 
 ## Business Answer
How might our data visualizations help county and state leadership or business owners in the US? What other data might we want to incorporate into an animated choropleth map to better understand the toll of the novel coronavirus in the United States?
