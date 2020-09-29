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
  - This notebook also identifies the top 10 oncology hospitals in the U.S. via an article at https://health.usnews.com/best-hospitals/rankings/cancer. The latitude/longitude coordinates for each of these hospitals was found via Google search.
  - The latitude/longitude coordinates of each of eight major urban centers were found via Google search.
  - The latitude and longitude coordinates of each EPA-designated Superfund Cleanup site were downloaded from the EPA's website at https://semspub.epa.gov/work/HQ/201261.pdf. The file had an embedded Excel spreadsheet that was converted into csv; only the name of the site, the latitude, and the longitude were kept.
  - Because one's access to quality food can influence one's risk for cancer, a series of features describing the food environment of each county is concatenated into the DataFrame. The source of this data is from research done by the USDA and is called the Food Environment Atlas, available from https://www.ers.usda.gov/data-products/food-environment-atlas/data-access-and-documentation-downloads/#August%202015%20Version .
  
 - Logarithmic and Exponential Transformations of the Feature Set (parts 1 through 4):
 https://github.com/danloew/Springboard-2nd-Capstone/blob/master/Cancer_LogExp_Expansion_1.ipynb
 https://github.com/danloew/Springboard-2nd-Capstone/blob/master/Cancer_LogExp_Expansion_2.ipynb
 https://github.com/danloew/Springboard-2nd-Capstone/blob/master/Cancer_LogExp_Expansion_3.ipynb
 https://github.com/danloew/Springboard-2nd-Capstone/blob/master/Cancer_LogExp_Expansion_4.ipynb
  - Logarithmic and exponential transformations of the feature set were tested for their contribution to the overall model’s accuracy, and added to the feature set if they increased this accuracy. 

