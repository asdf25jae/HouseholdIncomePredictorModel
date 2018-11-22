# HouseholdIncomePredictorModel
Household Income prediction model trained on the New York City Housing and Vacancy Survey data from 2017. 

Used R, R markdown in particular to train a multiple linear regression model 
based on income and housing/demographic data collected from the New York City Housing Vacancy Survey. 

Cleaned dataset by removing extreme outliers (incomes far above the average) and missing/truncated data (negative incomes)

Utilized Cook's distance to calculate extremity of outliers and removed all datapoints that were 4 times the mean Cook's distance.

Extracted salient features and tested variables through a partial F-test (with a null, full model) 
on the ANOVA table built in R. 

Used Leave One Out Cross Validation Error to calculate and compare ten different models
(with polynomial degree regression models included on the Age feature) and concluded that the multiple regression model with 
Age, Ethnic, Health, HeatBreaks, MiceRats and MaintenanceDef was the best fit to the data. 




Income : Response variable 
Gender : Male or Female 
Age : respondent's age (in years) 
Ethnic : self-reported race (Caucasian, African-American, Hispanic, Asian )
Health : self-assessment score of health
HeatBreaks : Number of heating equipment breakdowns since 2002 
MiceRats : presence of mice/rats in last 90 days 
CracksHoles : presence of cracks or holes in interior walls : Yes or No 
BrokenPlaster : presence of broken plaster on ceiling/interior walls : Yes or No 
WaterLeakage : presence of water leakage inside apartment : Yes, No 
MaintenanceDef : number of maintenance deficiencies between 2002 and 2005



