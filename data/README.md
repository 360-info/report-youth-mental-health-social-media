# `/data`

## Raw data  

### `ABS_Aus_2021.zip`  

This data are the 2021 Australian Bureau of Statistics General Community Profile. It was downloaded as a 'DataPack' via the following [interface](https://www.abs.gov.au/census/find-census-data/datapacks?release=2021&product=GCP&geography=AU&header=S)   

With direct download [link](https://www.abs.gov.au/census/find-census-data/datapacks/download/2021_GCP_AUS_for_AUS_short-header.zip)   

and renamed for readability. 

The analysis scripts automatically download and unzip this file if it doesn't exist. 


### `ABS_Geo_2021.zip`  

This data are the 2021 Australian Bureau of Statistics General Community Profile - Table G19. It was downloaded as a 'GeoPackage' via the following [interface](https://www.abs.gov.au/census/find-census-data/geopackages?release=2021&geography=AUS&table=G19&gda=GDA2020)   

With direct download [link](https://www.abs.gov.au/census/find-census-data/geopackages/download/Geopackage_2021_G19_AUS_GDA2020.zip)  

and renamed for readability. 

The analysis scripts automatically download and unzip this file if it doesn't exist. 
 
## `Data file Einstein.csv`  

This is the survey data collected in the below publication on FoMO and social media usage in adolescence.  

Danielle A. Einstein, Carol Dabb & Madeleine Fraser (2023) FoMO, but not self-compassion, moderates the link between social media use and anxiety in adolescence, Australian Journal of Psychology, 75:1, DOI: 10.1080/00049530.2023.2217961  

The data underlying this article are available in the Macquarie University Repository and can be accessed with https://doi.org/10.25949/20188298.v1


## `Variable labels Einstein.csv`  

This is the labels for the survey data collected in the below publication on FoMO and social media usage in adolescence.  

Danielle A. Einstein, Carol Dabb & Madeleine Fraser (2023) FoMO, but not self-compassion, moderates the link between social media use and anxiety in adolescence, Australian Journal of Psychology, 75:1, DOI: 10.1080/00049530.2023.2217961  

The data underlying this article are available in the Macquarie University Repository and can be accessed with https://doi.org/10.25949/20188298.v1


## Processed data  

### `mental_health_census.csv`   

These data are processed from the raw ABS data. It extracts counts and calculates proportions of those who identify 
as being diagnosed with a mental health condition in teh 2021 census.   

names         |type      |description |
|:-------------|:---------|:-----------|
|Age           |character | Age group           |
|Series        |character | Counts or Proportions           |
|men           |double    | Values for men           |
|women         |double    | Values for women           |
|men_tooltip   |character | Formatted values for tooltip           |
|women_tooltip |character | Formatted values for tooltip          |

### `mental_health_hotspot.geojson`  

These data take persons with mental health conditions, as recorded in the census. It subsets to only those aged 15-24 years old. The data are represented spatially at SA2 level.  

An analysis is performed to identify spatial clusters with LISA (Local Indicators for Spatial Association). The output of this analysis is captured in this `geoJSON` file for visualisation.  


|names            |type      |description |
|:----------------|:---------|:-----------|
|SA2_CODE_2021    |character | Statistical Area 2 Code           |
|SA2_NAME_2021    |character | Statistical Area 2 Name       |
|age              |character | Age group         |
|condition        |double    | Persons with reported mental health condition           |
|total            |double    | Total persons           |
|prop             |double    | Proportion of persons with reported menal health condition           |
|prop_lag         |double    | Spatial lagged values of `prop` using neighbouring areas       |
|cluster          |character | Spatial cluster           |
|prop_tooltip     |character | Formatted values for tooltip           |
|prop_lag_tooltip |character | Formatted values for tooltip            |


# FOMO 

https://doi.org/10.25949/20188298.v1

