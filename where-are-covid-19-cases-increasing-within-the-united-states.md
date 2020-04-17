---
description: >-
  Building a Plotly data animation to better visualize the spread of reported
  and confirmed COVID-19 cases within the United States.
---

# Where are COVID-19 Cases Increasing within the United States?

We'll use [plotly express](https://plotly.com/python/choropleth-maps/) to build an animated [choropleth map](https://www.arcgis.com/apps/MapJournal/index.html?appid=75eff041036d40cf8e70df99641004ca) that shows the number of cumulative confirmed COVID-19 cases per 1,000 residents in US counties, but first, we'll review some geospatial data analysis in Python by making a bubble map and a density heat map to showcase the number of cumulative COVID-19 confirmed cases in each US county on today's date. We'll use the data from April 15, 2020 fo this tutorial, but you can use the most updated data depending on the day that you conduct the analysis. 

### Choropleth Maps

For both of our data visualizations, we'll build **choropleth maps**, similar to the animated data visualization released on the JHU Coronavirus Resource Center website. Choropleth maps use different colors, shadings, or patterns in fixed geographic areas to showcase trends or regional differences in specific statistical measures such as socioeconomic, demographic, or other factors normalized over population, area, or some other feature. If we don't normalize the data in choropleth maps, larger numbers might look more significant even though the larger numbers may be due to larger populations or larger land areas.

We can make choropleth maps that include either [unclassified or classified data](https://www.arcgis.com/apps/MapJournal/index.html?appid=75eff041036d40cf8e70df99641004ca) ranges. Classified data means that we've pre-identified and associated different colors to specific data ranges. These can be more useful if we want to highlight specific data ranges \(e.g. geographic regions over or under a specific threshold\). 

Unclassified data means that our shaded or colored geographic shapes are pigmented according to a continuous color gradient range. These can be more useful if the data ranges change or if we want to showcase a more accurate range of data over a specific region.

Choropleth maps are different than [heatmaps](https://plotly.com/python/mapbox-density-heatmaps/) since we can see the data in discrete geographic areas instead of through continuous colors to show the density of points in given areas.



