# NYC Arrests
  
:statue_of_liberty: :police_car: :office:  
Exploration and visualization of arrests in New York City. 

## Tableau Dashboard
https://public.tableau.com/views/NYPDArrests/Arrests?:display_count=y&publish=yes&:origin=viz_share_link 

## Methodology and Summary
New York City arrest data was injested via the Socrata Open Data API (SODA) in Python.  The data was then processed to allow for easier analysis in Tableau.  Furthermore, GeoPandas was used to map each arrest to a neighborhood name based on its latitude and longitude.    
  
`See Jupyter Notebook for full details.`

## Data
  
Data  | NYC OpenData
------------- | -------------
Name  | NYPD Arrest Data (Year to Date)
Category  | Public Safety
Socrata domain  | data.cityofnewyork.us 
Socrata dataset identifier  | uip8-fykc 
Data range  | 2019-01-01 to 2019-09-30


Spatial Files  | NYC OpenData
------------- | -------------
1 | Neighborhood Tablulation Areas (NTA)
2  | Police Precincts


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
