## **Mapping Heat Vulnerability and Temperature Monitoring Sensor Suitability in Rhode Island**

### Abstract

Heat vulnerability across Rhode Island was evaluated at the block group level, integrating socio-demographic, housing, health, temperature, and landcover data to construct a heat vulnerability index (HVI), utilizing a principal component analysis. Results revealed substantial spatial heterogeneity, with higher vulnerability concentrated in urban centers, while rural areas generally showed lower risk. Suitability analysis for temperature sensors placement highlighted gaps in current monitoring infrastructure and identified optimal locations to enhance coverage, equity, and future adaptation. 

***

###	Methods and Data 

The study site included the entire state of Rhode Island, and analysis was performed on a block group level. Data was selected based on peer-reviewed literature and the Manware et al., 2022 study, and included demographic, economic, social, housing, diabetes, temperature, and landcover. Each was aggregated or calculated at the block group level.  

#### 2.1   Socio-Demographic and Housing Data
All socio-demographic and housing data were collected from the American Community Survey (ACS) 5-Year Estimates from 2018-2022. Variables included Hispanic or Latino, non-Hispanic African American or Black, elderly population, individuals living below poverty levels, individuals living alone, elderly and living alone, and limited English proficiency. Housing variables consisted of homes built before 1980. Manware et al., 2022 included foreign-born and disability variables, but due to data accessibility, these were excluded. The prevalence of diabetes was determined by gathering sex-specific county-level diabetes data from the Center for Disease Control (CDC). Data was combined with block group ACS age (individuals over 20) and sex distributions to estimate the number of diabetic adults per block group. Totals were summed and divided by the adult population to calculate 5-year averages.

#### 2.2   Air Temperature Data
2-m height air temperature data were collected from NASA’s Daymet (Version 4, 1 km2) dataset. 4-year averages of summer air temperature (June 1 to August 31, between 2018 and 2022) were calculated for each grid cell and aggregated at the block group level by using the area-weighted mean. The 20-year most frequent temperature (MFT) was determined for temperature data between January 1, 2002, and December 31, 2022. Data was obtained from NASA’s Daymet dataset, and monthly averages were extracted due to data availability. Modal temperatures were calculated per grid cell and aggregated at the block group level by using the area-weighted mean. Heat exposure was computed by taking the difference between summer averages and the 20-year MFT.  

#### 2.3   Landcover Variables
Landcover usage, tree canopy cover, and impervious surface percentages were obtained from the National Land Cover Database (NLCD). Proportion of land classified as “high density,” average tree canopy cover, and impervious surface. The fraction of non-green space was calculated by the relative area not covered by deciduous forest, evergreen forest, mixed forest, shrub/scrub, herbaceous, grassland, hay/pasture, cultivated crops, woody wetlands, and emergent herbaceous wetlands. All were determined on a block group level. The average enhanced vegetation index (EVI) was determined using NASA’s MOD13A2 Version 6 (MODIS, 250 m2) product. 4-year averages of summer months (June 1 to August 31, between 2018 and 2022) were calculated using 16-day scores and aggregated at the block group level by using the area-weighted mean.

#### 2.4   Calculating HVI
HVI was constructed using the methodology provided by Manware et al., 2022. Principal component analysis (PCA) with varimax rotation was used to reduce multicollinearity among the input variables and to identify the dominant dimensions of heat vulnerability. Three components were retained based on standard PCA criteria (Eigenvalue > 1, scree break, and cumulative variance explained), representing: (1) Socioeconomic & Environmental Exposure; (2) Elderly/Social Isolation; (3) Heat Exposure & Underlying Conditions. Normalized factor scores were rescaled from 1 to 6 based on deviation from the mean. Scores were summed to produce an index ranging from 3 to 18.

#### 2.5   ADI Scores
Area Deprivation Index (ADI) for Rhode Island was obtained from Neighborhood Atlas (CITE), to further assess heat disparities. ADI and HVI scores were compared on a block group basis, using a hexbin visualization.

#### 2.6   Station Locations 
Locations of temperature sensors and weather stations were collected from the National Oceanic and Atmospheric Administration (NOAA), the National Weather Service (NWS), and Brown University’s Network for Environmental Sensing & Technology (NEST). Stations were filtered out to those that collected air temperature (on a minute, hourly, or daily basis) and had long-term contemporary data (20+ years of continuous data, or actively recoding).

#### 2.7   Suitability for Sensor Placement
Selection of novel temperature sensing stations was accomplished on a state- and city-wide basis. State proposed sites guided by spatial rational (e.g., current placement of active stations) rather than quantitative criteria or analysis. Site suitability for additional temperature sensors in Providence was created using a multi-criteria analysis (MCA) based on four criteria: (1) distance to sidewalks, (2) distance to buildings, (3) tree canopy cover, and (4) solar radiation. Sidewalk, building footprint, and tree canopy cover spread were obtained from the Providence GIS Hub. Solar radiation (e.g., aspect) was calculated using a digital elevation model (DEM) collected from the U.S. Geological Survey (USGS). Criteria were determined using guidelines provided by the NWS (NWS, 2016). Areas within direct proximity to sidewalks (considering potential utility or light poles available for sensor attachment, and accessibility factor), away from buildings, not directly under canopy spread, and south-facing (for optimal direct sunlight) were scaled as most preferable. All four components were equally weighed. Final selection for new locations considered suitability results, in addition to current station placement and HVI scores.
