Phenology of three vegetation communities in the Santa Clara River watershed

This repository contains an analysis of the phenology, or life cycle events, of three vegetation communities in the Santa Clara River watershed. In this analysis, we compute monthly NDVI values between June 2018 and July 2019 from Landsat satellite scenes. We then compare the monthly NDVI values
across 5 study sites near the Santa Clara River that represent the following types of vegetation:

-   riparian forest

-   grasslands

-   chaparral shrublands

The structure and contents of the repository are:

    geospatial-analysis-2021-houston-blackouts
    │   README.md                               
    │
    └───data/
    |   │   landsat_20180612.tif      #6/12/2018 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20180815.tif      #8/15/2018 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20181018.tif      #10/18/2018 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20181103.tif      #11/3/2018 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20190122.tif      #1/22/2019 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20190223.tif      #2/23/2019 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20190412.tif      #04/12/2019 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   │   landsat_20190701.tif      #7/1/2019 surface reflectance scene from OLI sensor of the [Landsat Operational Land Imager](https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/)
    |   |   study_sites.dbf       #shapefiles of Santa Clara River watershed study sites from [Dr. Christopher Kibler] (https://ckibler.com/) of the University of California, Santa Barbara 
    |   |   study_sites.prj       #shapefiles of Santa Clara River watershed study sites from [Dr. Christopher Kibler] (https://ckibler.com/) of the University of California, Santa Barbara    
    |   |   study_sites.shp       #shapefiles of Santa Clara River watershed study sites from [Dr. Christopher Kibler] (https://ckibler.com/) of the University of California, Santa Barbara 
    |   |   study_sites.shx       #shapefiles of Santa Clara River watershed study sites from [Dr. Christopher Kibler] (https://ckibler.com/) of the University of California, Santa Barbara 
    │
    └───figures/
    |   |   seasonal_ndvi.png       #timeseries of NDVI over time for all study sites
    |
    └───scripts/ 
    │   |   analyze_plant_phenology.Rmd file        #analysis markdown file
    │   │   analyze_plant_phenology.html file       #analysis HTML file

All the data used in the exercise are included in the repository. Descriptions of the original data sources are shown below: 

**Landsat Operational Land Imager (OLI sensor)**\

-   8 pre-processed scenes\
    -   Level 2 surface reflectance products\
    -   erroneous values were set to NA\
    -   scale factor set to 100\
    -   bands 2-7\
    -   dates in filenname\

**Study sites**

-   polygons representing sites\
    - study_site: character string with plant type
    
A summary figure from the analysis is shown below:
![Alt Text](https://github.com/kristinart/plant-phenology-santa-clara-river/blob/main/figures/seasonal_ndvi.png)
