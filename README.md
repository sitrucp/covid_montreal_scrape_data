**Montreal Confirmed COVID-19 Cases By City Neighbourhoods**

This repository contains Python code that is used to get confirmed COVID-19 case counts for Montreal which is Canada's "covid hotspot". 

The data for this comes from the <a href ="https://santemontreal.qc.ca/en/public/coronavirus-covid-19/">Quebec Health Montreal website</a> which has a regularly updated table of confirmed cases counts by Montreal city neighbourhoods. 

To obtain this tabular data in an automated and scheduled manner this web server based Python cron job was created. The Python code also uploads the data to an AWS S3 bucket which is visualization data source.

The Python script uses BeautifulSoup4, Requests and Pandas to retrieve and transform webpage table data and results in a json data file "montreal_confirmed_cases.json" which is the data source for the Leaflet choropleth map.

The Leaflet choropleth map is here: <a href ="https://sitrucp.github.io/canada_covid_health_regions/montreal/montreal.html"></a>

More details on Leaflet map visualization are here: <a href ="https://github.com/sitrucp/canada_covid_health_regions"></a>








