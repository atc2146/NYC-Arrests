# NYC Arrests
  
:statue_of_liberty: :police_car: :office:  
Exploration and visualization of arrests in New York City

## Tableau Dashboard
https://public.tableau.com/views/NYPDArrests/Arrests?:display_count=y&publish=yes&:origin=viz_share_link 

## Methodology and Summary
New York City arrest data from NYC OpenData was ingested via the Socrata Open Data API (SODA) in Python.  The data was then processed to allow for easier analysis in Tableau.  GeoPandas was used to map each arrest to a neighborhood name based on its latitude and longitude.    
  
`See Jupyter Notebook for full details.`

## Data
  
Data File | Name  | Category | Socrata domain | Socrata dataset identifier | Data range | Update frequency
------------- | ------------- |------------- | ------------- |------------- | ------------- | ------------- 
1D | NYPD Arrest Data (Year to Date)  | Public Safety | data.cityofnewyork.us  | uip8-fykc | Year to date | Quarterly
2D | NYPD Arrest Data (Historic)  | Public Safety | data.cityofnewyork.us  | 8h9b-rp9u | 2006 to end of previous calendar year | Annually


Spatial File  | NYC OpenData
------------- | -------------
1S | Neighborhood Tablulation Areas (NTA)
2S  | Police Precincts
  

File  | URL
------------- | -------------
1D | https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc
2D  | https://data.cityofnewyork.us/Public-Safety/NYPD-Arrests-Data-Historic-/8h9b-rp9u
1S | https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq
2S  | https://data.cityofnewyork.us/Public-Safety/Police-Precincts/78dh-3ptz


## Resources

 * Socrata Open Data API: https://github.com/xmunoz/sodapy  
 * Socrata Dev: https://dev.socrata.com/  
 * NYC OpenData: https://opendata.cityofnewyork.us/  
 * Time Series Analysis: https://dev.socrata.com/blog/2019/10/07/time-series-analysis-with-jupyter-notebooks-and-socrata.html  
 * Pandas, Numpy, GeoPandas  

## Future Updates
 * Include more data (data from 2018 and before)  
 * Visualizations for YoY and MoM changes 

## Author
Alex Chung
