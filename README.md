# Springboard-2nd-Capstone
Repository with Full Code, Report, and Slide Deck for Daniel Loew's second Springboard capstone project

Title: "Predicting Cancer Mortality in United States Counties: 2015"

This project uses publicly available data from [sources] to build predictive machine learning regression models of cancer mortality at the U.S. county level, providing Ridge  Regression coefficients which illuminate the features that have the strongest statistical relationship with cancer mortality rates. The Jupyter notebooks, data sources, technical requirements for reproducing the results, and reports for this project are specified below. The results of this project, including evaluation metrics of the machine learning models and Ridge Regression coefficients, are reported in the Overall Capstone Project Report linked to below.

The x Jupyter notebooks that are needed to run the project are located at the following links:

- Data Cleaning:
  https://github.com/danloew/Springboard-2nd-Capstone/blob/master/Cancer_Data_Cleaning.ipynb
  
  - The file name is 'Cancer_Data_Cleaning.ipynb'.
  - This notebook uses a data set of socioeconomic indicators and cancer mortality rates for the year 2015 for 3,047 out of 3,141 total U.S. counties (97%    of all U.S. counties and county equivalents), which came came pre-assembled as a data science challenge from three sources: the American Community Survey (census.gov), clinicaltrials.gov, and cancer.gov. It was downloaded from https://data.world/exercises/linear-regression-exercise-1​. The assemblage process can be examined at ​https://data.world/nrippner/cancer-trials​. The data dictionaries are located at https://data.world/exercises/linear-regression-exercise-1/workspace/data-dictionary​. In order to access these files, one needs to set up a free account for data.world.
  - This notebook also uses a United States Census data set of latitude/longitude centroids for all United States counties, as well as separate features for the state that each county is in, the landmass square mileage for each county, and the water area square mileage, all of which were concatenated with the primary data set using pandas' .concat() method. This data set is called '2019_Gaz_counties_national.csv', and was downloaded from https://www2.census.gov/geo/docs/maps-data/data/gazetteer/2019_Gazetteer/2019_Gaz_counties_national.zip. 38 counties in the original data set were not in the Census' data set, so their latitude/longitude centroids and landmass/water area square mileage were looked up via Google.
  - This notebook also uses a 
    
