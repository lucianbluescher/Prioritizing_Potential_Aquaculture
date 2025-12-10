# Prioritizing Potential Aquaculture
<img width="1024" height="683" alt="image" src="https://github.com/user-attachments/assets/133f8bb5-d1c9-4007-be73-185dfbc13eab" />

Image Credits: (Jane March, The Road Ahead for Sustainable Aquaculture)[https://earth.org/sustainable-aquaculture/]

‌

### Lucian Scher |  11/26/25

## Purpose
Marine aquaculture offers a sustainable protein source with minimal ocean footprint. This repository contains a project creates a function that uses a species sea surface temperature and depth thresholds and returns a map of optimal West Coast U.S. Exclusive Economic Zone locations for the given species in order to identify the most suitable aquaculture areas. This analysis uses the function to look at oysters generally, Olympia Oysters and Red Abalone species 

## Contents 
Important files included in this repository is all the data required to run the analysis located in the data folder and Prioritizing_Potential_Aquaculture.qmd, a markdown that can be run to see the function being used. The markdown also contains all neccessary data preparation, processing and the complete function code with a Roxygen skeleton. 

## Data

Parameters for species analysis were accessed 11/26/25 and can be found at:
  -   SeaLifeBase. (2023). Sealifebase.ca. https://www.sealifebase.ca/search.php
Specific links to each species can be found in the .qmd.

Sea Surface Temperature (SST) Data accessed 11/25/25 was originally generated for the years 2008-2012 from:
 -    ‌NOAA Coral Reef Watch Daily 5km Satellite Coral Bleaching Heat Stress SST Anomaly Product (Version 3.1). (2018). Noaa.gov. https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php

‌Bathymetry (Depth) data accessed 11/25/25 is originally from:
   -  Gridded Bathymetry Data. (2025). GEBCO. https://www.gebco.net/data-products/gridded-bathymetry-data#area

For mapping the west coast we use the "rnaturalearth' package installed 11/25/25:
    - ropensci/rnaturalearth: An R package to hold and facilitate interaction with natural earth map data (2023, December 15). GitHub. https://github.com/ropensci/rnaturalearth

‌
‌

## File Structure
```
EDS223-HW3
└─── README.md
└─── qmd/Rmd/Proj files
└─── Prioritizing_Potential_Aquaculture.qmd
|   .gitignore
    └───data
        └─── wc_regions_clean.shp
        └─── depth.tif
        └─── average_annual_sst_2008.tif
        └─── average_annual_sst_2009.tif
        └─── average_annual_sst_2010.tif
        └─── average_annual_sst_2011.tif
        └─── average_annual_sst_2012.tif
```

## Acknowledgments
This project was a homework assignment for the fall 2025 course, Geospatial Analysis & Remote Sensing (EDS 223). A part of the Master of Environmental Data Science (MEDS) program at UCSB's Bren school of Environmental Science & Management. The assigment was created by Ruth Oliver and administered by Annie Adams. This project was extremely enjoyable thanks to both of them. Additionally, the project was inspried by Rebecca R. Gentry's paper [*Mapping the global potential for marine aquaculture*](https://www.nature.com/articles/s41559-017-0257-9) which mapped marine aquaculture potential and laid the groundwork for this assignment.

