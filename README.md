# BrainStation-Capstone-Project
Capstone project completed as a part of the Data Science Diploma program requirements.

Predicting CO2 Flux and Storage in Boreal Forests

This project aims to use data science modeling tools on the available data to capture the trends of the CO2 exchange (flux) and stocks 
(storage) for the Boreal Forests. 

Disclaimer:

This study presented here is only an initial attempt to capture the CO2 flux and storage trends in the Boreal Forests modeled using 
the BOREAS datasets from the 1990s, which needs to be updated to current data, when available.

Model trends are only as good as the data used, which means better standardized data can increase prediction accuracy.

Please do not use these notebook for publishing. Further research and expert opinions are needed to validate the results.

Background of the Study:
Recent studies by Natural Resources Defense Council, In. (NRDC), Environmental Defense Canada (EDC) and Nature Canada, have stated that 
the Carbon Budget Model (CBM-CFS3) used to evaluate the forest carbon stocks and stock changes for the past or into the future, has 
recently shown to be underestimating the cost of clear-out logging, especially in accounting for the greenhouse gas emissions due to:
i)	soil respiration emissions increase due to soil disturbance during and after logging and due to left over tree biomass 
	decomposition 
ii)	reduction in carbon stocks and flux due to areas that don’t regrow i.e., soil carbon (C) loss and decreased efficiency of CO2 
	absorption/sequestration

Given that there are large data measurements to model the carbon sequestration (absorption and emission of C) in the Boreal Forests 
ecosystem, the complexity involved in applying manual statistical analysis or linear models on large datasets can lead to failure in 
capturing important C trends. Consequently, to develop a model/method that can accurately capture and estimate the changes in the C trends due to 
advertent and inadvertent impacts of human activities, the current advances in data science tools, and techniques for organizing and 
analyzing large amounts of data needs to be effectively employed by environmental researchers and policy makers alike. 

Dataset:
Source of the Data and dataset: (data used and schema)
The Boreal Ecosystem-Atmosphere Study (BOREAS) was a large-scale international interdisciplinary experiment (from 1993-1996) in the boreal 
forests of central Canada. It focused on improving our understanding of the exchanges CO2 and trace gases between the boreal forest and 
the lower atmosphere. A primary objective of BOREAS was to collect the data needed to improve computer simulation models so that scientists
can anticipate the effects of global change on the biome.

Two study sites were selected - the Northern (NSA) and Southern Study Area (SSA) in Manitoba and near Prince Albert, Saskatchewan, respectively. Also, for this study purpose only vegetation cover was narrowed to Old Black Spruce (OBS). These sites have been mapped using Tableau.

In the BOREAS website, I mainly worked on the following datasets (all other datasets downloaded/worked on are provided in the ‘Read Me’ file):
•	BOREAS TF-03 NSA-OBS Tower Flux, Meteorological, and Soil Temperature Data
•	BOREAS TE-01 CO2 and CH4 Flux Data over the SSA-OBS Site 
•	BOREAS TF-07 SSA-OBS Tower Flux and Meteorological Data

Data Schema – Each data file listed above had its own structure and schema, which were kept mostly similar between the two study sites. 
Please check the comp folder 'def' text files to know more about the schema of each data file.

Contents of the Project File Submitted:

#BORIS_Coordinates_Input_Output_Code_Files
In an effort to properly document the sites and areas where data were collected, personnel of the BOReal Ecosystem-Atmosphere Study 
(BOREAS) Information System (BORIS) obtained and compiled geographic coordinate and other site information from several sources throughout 
the experiment period. 
The folder contains: 
1. Boreal_Coords.ipynb - A python notebook used to read file and process it into a excel file format and reduce the columns and the rows to 
show only filtered data points for NSA-OBS and SSA-OBS locations. 
2.Boreal_Site_Coords.xlsx (Converted from .csv output) - excel file output from the python notebook that will be imported in the Tableau 
workbook.
3. Tableau Workbook (NSA_and_SSA_site_locations.twb)  - Consists of data points in the 'Boreal_Site_Coords.xlsx' plotted on the map.

#data
Consists of two input 'Tower_Flux_Meter_NSA_OBS' and 'Tower_Flux_Meter_SSA_OBS' csv files that were read in the python notebook 
'Flux_Conc_Data_Workbook.ipynb' for cleaning, modeling and visualization
Also, a folder containing the .csv input files data collection, range, units, description details documented by the BOREAS study data 
collection teams.
The 1994 NSA-OBS and the SSA-OBS combined CO2 flux and storage csv file is also available in the data folder 

#Flux_Conc_Data_Workbook
Jupyter notebook wherein the input files were read, preprocessed, cleaned, filtered,  explored, combined, modeled for CO2 flux and 
storage trends and model prediction analysis and visualization was completed.


