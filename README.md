Similarities-Between-Counties

This project was for DS5230 Unsupervised Machine Learning at Northeastern University Fall 2021. The aim of this project was to use unsupervised machine learning algorithms to determine which demographic, geographic, and economic features of a county are most important in determing whether two US countieis will be similar or not. 

The Dataset folder contains all the datasets and the Project Code file contains all of the code used for this project. 

acs2017_county_data.csv and acs2015_county_data.csv are the DP03 and DP05 tables of the American Community Survey for that year. uscounties.csv is the latitude and longitude of each US county or county equivalent. PuertoRicoLocationData.csv is the latitude and longitude values of the 78 municipalities of Puerto Rico. us census bureau regions and divisions.csv is the region and division that each state plus D.C. is in according to the US Census Bureau with Puerto Rico added. 

The file EDA Code.rmd is the file used to read in all of the datasets and join the datasets together based on county name or by state name. 

The file Forming Groups for MBA.rmd is the file used to turn all of the numeric columns for the 2017 full county dataset and the additional columns such as max gender and max race. 

The file MBA Code.rmd is the code used to run MBA on the newly created dataset created in Forming Groups for MBA.rmd. However, only 15 of the 44 columns of the new_2017_data were used. The 15 columns were TotalPop, IncomePerCap, IncomePerCapErr, Poverty, MeanCommute, Lat, Long, Gender Favored, Max Ethnicity, VotingAgeCitizen Percent, Max Employment Source, Max Travel Source, EmployedPercent, Max Work Source, and Unemployment.

The file UML_Project.ipynb contains code loading in and fortmatting the data, as well as normalizing it to the unit hyper-cube. Then it is cleaned (a couple of NaN values removed) and used in PCA and t-SNE algorithms in order to help analyze the data in low dimensions. This is where many of the plots are created as well. 

The file Ethan_code.ipynb contains code for loading in the full datasets, normalizing the datasets. The file also includes the code for Ridge and Lasso regression that was tried to find the most important features as well as clustering techniques used for both the full dataset and the dataset without Alaska, Hawaii, and Puerto Rico as well as without location.
