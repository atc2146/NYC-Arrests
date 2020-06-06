# Crime in NYC

:statue_of_liberty: :police_car: :office:  
Exploration and visualization of arrests/crime in New York City

## Tableau Dashboard

Find the [Tableau Dashboard here](https://public.tableau.com/views/NYPDArrests/Arrests?:display_count=y&publish=yes&:origin=viz_share_link "Tableau Public - Alex Chung | Crime in NYC").  

Find my other dashboards on [Tableau Public](https://public.tableau.com/profile/alex.chung#!/ "Tableau Public - Alex Chung").

## Methodology and Summary
New York City arrest data from NYC OpenData was ingested via the Socrata Open Data API (SODA) in Python.  The data was then processed using Pandas/NumPy to allow for easier analysis in Tableau.  Using spatial files (.shp), GeoPandas was used to map each arrest to a neighborhood name based on its latitude and longitude (i.e. reverse geocoding).  

Data was [scraped](nyc-arrests-precinct-scrape.ipynb) using BeautifulSoup from the NYC Gov site to get information regarding Police Precincts.  

`See Jupyter Notebooks for full details.`

## Data

Data File | Name  | Category | Socrata domain | Socrata dataset identifier | Data range | Update frequency
------------- | ------------- |------------- | ------------- |------------- | ------------- | -------------
[1D](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc) | NYPD Arrest Data (Year to Date)  | Public Safety | data.cityofnewyork.us  | uip8-fykc | Year to date | Quarterly
[2D](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrests-Data-Historic-/8h9b-rp9u) | NYPD Arrest Data (Historic)  | Public Safety | data.cityofnewyork.us  | 8h9b-rp9u | 2006 to end of previous calendar year | Annually


Spatial File  | Name
------------- | -------------
[1S](https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq) | Neighborhood Tablulation Areas (NTA)
[2S](https://data.cityofnewyork.us/Public-Safety/Police-Precincts/78dh-3ptz) | Police Precincts

Other  | Name
------------- | -------------
[O1](https://www1.nyc.gov/site/nypd/bureaus/patrol/precincts-landing.page) | NYPD Precincts  



File  | URL
------------- | -------------
1D | https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc
2D  | https://data.cityofnewyork.us/Public-Safety/NYPD-Arrests-Data-Historic-/8h9b-rp9u
1S | https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq
2S  | https://data.cityofnewyork.us/Public-Safety/Police-Precincts/78dh-3ptz
O1  | https://www1.nyc.gov/site/nypd/bureaus/patrol/precincts-landing.page

For this project, data was pulled from the start of 2017 to the end of the previous quarter of the current calendar year.   Note: data is available from 2006 onwards.


## Resources

 * [Socrata Open Data API](https://github.com/xmunoz/sodapy)  
 * [Socrata Dev](https://dev.socrata.com/)  
 * [NYC OpenData](https://opendata.cityofnewyork.us/)  
 * [Time Series Analysis](https://dev.socrata.com/blog/2019/10/07/time-series-analysis-with-jupyter-notebooks-and-socrata.html)  
 * Python Packages: Pandas, NumPy, GeoPandas  

## Extensions
 * Optimize data and data pull
 * Add ranks for each area in each map layer
 * Visualizations for YoY and MoM changes

## Author
Alex Chung
