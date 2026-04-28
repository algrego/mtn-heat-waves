# Mountain Heat Waves
## GEOG 4563-5563 Final Project - SPRING 2026

> Authors: Alison Gregory (alison.gregory@colorado.edu) & Raini Helmstadter (raini.helmstadter@colorado.edu)

### Project Description 
This project looks at data from the CDC's social vulnerability index (SVI), the MACAv2 Climate Data (futures and historical), and CDC county and census tract data to understand how climate change and socio-economic variables of ski town communities. This exploratory analysis looked at the regions around Aspen/Vail - Colorado, Big Sky - Montana, and Jackson Hole - Wyoming. 

### DOI
[![DOI](https://sandbox.zenodo.org/badge/1210815773.svg)](https://handle.test.datacite.org/10.5072/zenodo.494154)


### Data Sources


#### Location Data
CDC Census Tract Data 
- Colorado
Aspen/Vail county codes: “037”, “097”
- Montana
Big Sky county codes: “031”, “057” 
- Wyoming
Jackson Hole county code: “039”

*Note: Future work may look at CDC Census Tract Data rather than County codes to get a higher resolution of data.*
 

#### Climate Data

[MACAv2](https://climate.northwestknowledge.net/MACA/data_portal.php) 
Summer and Winter average of Maximum Air Temperature (tasmax) 
- Historical (1990 - 2005)
- Future RCP 4.5 (2046 - 2065)
We can use climate data to calculate potential heatwaves/other extreme events, as well as Summer and Winter precipitation totals (same time period as tasmax). We might need to figure out how to calculate potential flood events in the models and make flood/snowpack calculations
 
#### Socioeconomic Data

[CDC Social Vulnerability Data](https://www.atsdr.cdc.gov/place-health/php/svi/svi-interactive-map.html)


### Requirements and How to Run the Code
1. This notebook (mtn-heat-waves.ipynb) was run using the earth-data-analytics kernel (Python 3.11.14). Various imported python packages will be needed to interpret the raster data, download files, and visualize the data.
2. Run the notebook as normal

3. **Important!** In section 2 (Download Social Vulnerability Data), there is not a publicly available API to download the files directly from the web. To ensure this portion of the code runs successfull you need to do the following steps
- [x] Go directly to [SVI Data & Documentation Download](https://www.atsdr.cdc.gov/place-health/php/svi/svi-data-documentation-download.html).
- [x] In the dropdown menu select the year (2022), the geography (United States), ansd the geography type (Counties)
- [x] Ensure that the file type ESRI GEodatabase (map data) is selected and press "Go"
- [x] Save that folder into the 'data_dir'. In this notebook it is located at 
'data_dir = os.path.join(pathlib.Path.home(), "Earth Data Analytics", "Mtn-Heat-Waves", "data")'

### Key Findings and Next Steps

 
