Rows: 34990 (62 US cities)
Columns: 29 [cities, year, pollen type, week in year, pollen count (grains per cubic meter), number of times observed per week, state, county code, county name, zipcode, arsenic, cadmium, chromium, lead, manganese, nickel, zinc, daily average temperature, daily average high, daily average low, total amount of precip, average daily humidity, average daily dewpoint, average daily wind, average of daily max winds, average daily sunlight, temp from previous week, average precip from prev week, avg humidity from prev week']
Sources:
1. pollen weekly dataset
 https://data.cdc.gov/National-Center-for-Environmental-Health/Weekly-Grouped-Pollen-Concentrations-Trees-and-Wee/bgxp-nxmn/about_data
 Data collected by the National Allergy Bureau and processed by the Division of Environmental Health Science and Practice (DEHSP), National Center for Environmental Health (NCEH), and CDC
 Weekly pollen concentrations of trees and weeds for 116 US cities from 2003-2024

2. heavy metal weekly dataset
   https://aqs.epa.gov/aqsweb/airdata/download_files.html#Daily
   Data by the EPA's Air Quality System
   Weekly speciation (breaking down of PM2.5 into heavy metals, chemical ingredients) of each year from 2003-2024 for the select US cities for arsenic, cadmium, chromium, lead, manganese, nickel, zinc

3. weather weekly dataset
   https://power.larc.nasa.gov/
   Data by NASA POWER
   Weekly temp, rainfall, humidity, dew point, wind, sunlight in above US counties from 2003-2024

Because the heavy metal data was limited, after merging the pollen and heavy metal dataset, the number of counties went from 102 to 62. However, this limitation is minimal because there is still thousands of rows of data to analyze. 
Another potential issue to keep in mind is that the weather and heavy metal data comes from county reports: there are 52 cities in the final dataset throughout 62 different counties. This means 2 sites in the same county will have the same weather and heavy metal data which is a problem to keep in mind when splitting data.
   
