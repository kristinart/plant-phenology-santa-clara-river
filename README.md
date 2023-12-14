# plant-phenology-santa-clara-river




# Overview
Phenology is the timing of life history events. Important phenological events for plants involve the growth of leaves, flowering, and senescence (death of leaves). Plants species adapt the timing of these events to local climate conditions to ensure successful reproduction. Subsequently, animal species often adapt their phenology to take advantage of food availability. As the climate shifts this synchronization is being thrown out of whack. Shifts in phenology are therefore a common yardstick of understanding how and if ecosystems are adjusting to climate change.\

Plant species may employ the following phenological strategies:\

-   winter deciduous: lose leaves in the winter, grow new leaves in the spring\
-   drought deciduous: lose leaves in the summer when water is limited\
-   evergreen: maintain leaves yearround\

credit: this lab is based on a materials developed by Chris Kibler.

# Task
In this lab we are analyzing plant phenology near the Santa Clara River which flows from Santa Clarita to Ventura. We will investigate the phenology of the following plant communities:\

-   riparian forests: grow along the river, dominated by winter deciduous cottonwood and willow trees\
-   grasslands: grow in openspaces, dominated by drought deciduous grasses\
-   chaparral shrublands: grow in more arid habitats, dominated by evergreen shrubs\

To investigate the phenology of these plant communities we will a time series of Landsat imagery and polygons identifying the locations of study sites within each plant community.\

## Data

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
    
## Summary of approach
-   Convert spectral relfectance into a measure of vegetation productivity (NDVI)
-   Calulate NDVI throughout the year
-   Summarize NDVI values within vegetation communities
-   Visualize changes in NDVI within vegetation communities

# Workflow


![Alt Text](https://github.com/kristinart/plant-phenology-santa-clara-river/blob/main/figures/seasonal_ndvi.png)
