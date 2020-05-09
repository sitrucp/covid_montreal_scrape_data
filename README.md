**Montreal Confirmed COVID-19 Cases By City Neighbourhoods**

This repository contains Python code used to get and transform confirmed COVID-19 case counts from the <a href ="https://santemontreal.qc.ca/en/public/coronavirus-covid-19/">Quebec Health Montreal website</a> which has a regularly updated table of confirmed cases counts by Montreal city neighbourhoods. 

The scraped data is used in a Leaflet choropleth map visualization <a href ="https://sitrucp.github.io/canada_covid_health_regions/montreal/montreal.html">https://sitrucp.github.io/canada_covid_health_regions/montreal/montreal.html</a>

A web server based cron job is employed to retrieve and transform the Quebec Health Montreal website data in an automated and scheduled manner, and upload the data to an AWS S3 bucket which is visualization's data source.

The Python script uses BeautifulSoup4, Requests and Pandas to retrieve and transform webpage table data and results in a json data file "montreal_confirmed_cases.json" which is the data source for the Leaflet choropleth map.

More details on this web scraping and the Leaflet map visualization can be found:

Blog post describing the code and background in bit more detail <a href ="https://009co.com/?p=1009">Scraping public health web page to get data</a>

Blog post describing the code and background in bit more detail <a href ="https://009co.com/?p=963">Choropleth map of Canada COVID-19 cases by health region using Leaflet and D3</a>

Github repository <a href ="https://github.com/sitrucp/canada_covid_health_regions">https://github.com/sitrucp/canada_covid_health_regions</a>








