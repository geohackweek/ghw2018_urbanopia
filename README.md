# ghw2018_urbanopia
Public version of the private urbanopia_geohackweek_2018 repo. The main repo is private to avoid issues with PII. The main repo is at https://github.com/LucieCBurgess/Urbanopia_geohackweek2018

## Urbanopia: exploring the relationship between mental health and the built and social urban environment 
using land-use raster data and OpenStreetMap data

## Collaborators:      
@edwardlxb @ianpdavies @LucieCBurgess @norlab @tz222 @youngjc2

## The problem
The Urban Mind dataset contains data on mental state in relation to perceptions of the built and social environment. Observations are geotagged which allows context to be developed from the geotagged points. During the hackweek we would like to explore two main problems:  
1. The relationship between perceptions of planning inclusivity and street features (such as the availability of street seating, pedestrian crossings, street trees) from OpenStreetMap data
2. The relationship between perceptions of greenness, actual greenness and mental state using NVDI raster data

## Application Example
This work is useful to explain the relationship between perceptions of the urban environment and mental health. 

## Sample data
The Urban Mind data is only available to research collaborators on signature of a data sharing agreement. Tags relating to the location data (e.g. home, work) have been removed to preserve participants' privacy, even though the data are anonymous.
OpenStreetMap data can be downloaded using several libraries and methods - see our Slack channel for links, e.g. 
https://automating-gis-processes.github.io/2017/lessons/L7/retrieve-osm-data.html  
https://geoffboeing.com/2016/11/osmnx-python-street-networks/

We are trying to access the following data from the Centre for Ecology and Hydrology in the UK:
25m x 25m raster data on land cover, classified into 25 different types
https://www.ceh.ac.uk/services/land-cover-map-2015#obtain 

## Specific questions
Download and use OSM data from geojson format to geopandas, and extract data on specific tags such as street features.
Extract data on tree cover/ greenness from NDVI raster images.
Develop analytical models to correlate these data with mental states from participants at geotagged locations.

## Existing methods/ proposed methods and tools
Modelling:
PCA, spatially-weighted regression, spatial random forest for classification.
Note the data are self-correlated so GLMMs or Bayesian GLMMs could also be used.

## Building from what you learn at geohackweek, what new approaches would you like to try to implement?
See above. It would also be useful to develop a simple 'front end' to navigate the resulting notebooks and documentation, perhaps using Sphinx/ read_the_docs or Github pages.

## Background reading
United Nations (2016) The world’s cities in 2016 - data booklet.   
Vassos E, Pedersen CB, Murray RM, et al. (2012) Meta-Analysis of the Association of Urbanicity With Schizophrenia. Schizophrenia bulletin 38(6). Oxford University Press: 1118–1123.   
Andrade LH, Wang Y-P, Andreoni S, et al. (2012) Mental disorders in megacities: findings from the São Paulo megacity mental health survey, Brazil. PloS one 7(2): e31879.   
Cattell V, Dines N, Gesler W, et al. (2008) Mingling, observing, and lingering: everyday public spaces and their implications for well-being and social relations. Health & place 14(3): 544–561   
Sarkar C and Webster C (2017) Healthy Cities of Tomorrow: the Case for Large Scale Built Environment-Health Studies. Journal of Urban Health 94(1): 4–19.   
Bakolis I, Hammoud R, Smythe M, et al. (2018) Urban Mind: Using Smartphone Technologies to Investigate the Impact of Nature on Mental Well-Being in Real Time. Bioscience 68(2): 134–145.  


