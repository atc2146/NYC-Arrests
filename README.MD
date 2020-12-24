# :statue_of_liberty: Crime in NYC

Exploration and visualization of arrests/crime in New York City.  

## :bar_chart: Tableau Dashboard 

Find the [Tableau Dashboard here](https://public.tableau.com/views/NYPDArrests/Arrests?:display_count=y&publish=yes&:origin=viz_share_link "Tableau Public - Alex Chung | Crime in NYC").  

## :chart_with_upwards_trend: Methodology
New York City arrest data from NYC OpenData was ingested via the Socrata Open Data API (SODA) in Python.  The data was then processed using Pandas/NumPy to allow for easier analysis in Tableau.  Using spatial files (.shp), GeoPandas was used to map each arrest to a neighborhood name based on its latitude and longitude (i.e. reverse geocoding).  

To get information regarding police precincts, data was scraped using BeautifulSoup from the NYC Gov. site.  

See [code](Code/) in Jupyter Notebooks for full details.

## :floppy_disk: Data

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


For this project, data was pulled from the start of 2018 to the end of the previous quarter of the current calendar year.  

Note: Data is available from 2006 onwards.  Last quarter's data may not be completely accurate due to lag from NYPD to the NYC OpenData database.


## :books: Resources

 * [Socrata Open Data API](https://github.com/xmunoz/sodapy)  
 * [Socrata Dev](https://dev.socrata.com/)  
 * [NYC OpenData](https://opendata.cityofnewyork.us/)  
 * [Time Series Analysis](https://dev.socrata.com/blog/2019/10/07/time-series-analysis-with-jupyter-notebooks-and-socrata.html)  
 * Python Packages: Pandas, NumPy, GeoPandas  

## :pencil: Extensions
 * Add crime rate toggle to map (i.e. number of crimes/population)
 * Visualizations for YoY and MoM changes

## :wave: Author
Alex Chung
