# COVID-19 Prediction Model by U.S. County: High, Medium or Low Risk (as of August 18th, 2020)
The goal of this project was to create a model that could predict a county's risk for COVID-19 cases and deaths based on and assessment of county variables and the county's most recent peak value of COVID-19 cases and deaths. 

Data classification based on assigned label of "High", "Medium" or "Low" risk. 

Variables included: 
- Population Density
- Population Ethnicity: black, hispanic, white, asian, american indian
- Median Income
- Commuters by Public Transportation
- Social Distancing Scores

# Data Sources
- Johns Hopkins University - latest numbers for COVID-19 deaths and cases: https://github.com/CSSEGISandData/COVID-19
- US Census:https://console.cloud.google.com/marketplace/product/united-states-census-bureau/us-census-data?project=data-mining-project-280712 
- Unacast - Social Distancing score cards: https://www.unacast.com/covid19/social-distancing-scoreboard
- ARCGis - Population density information: https://hub.arcgis.com/datasets/fab7849b55d54f0f8f246605f6ee9306

# Results and R Code
Visual analysis and R code are detailed in this webpage: https://starrc.github.io/covid19_prediction/

# File Explanations
1. Deaths Prediction results by county: deaths_predictor_rules.csv
2. Cases Prediction results by county: cases_predictor_rules.csv
3. Raw R Code: 
    - Calculate Peak Cases and Deaths values by County and Map: peak.Rmd
    - Deaths Prediction Model: deaths.Rmd
    - Cases Prediction Model: cases.Rmd
4. Population Density Data: USA_Population_Density.csv
5. Social Distancing Scorecards: Unacast_Social_Distancing_Score.csv

# Model Instructions and Requirements
1. Run peak.Rmd file
   - Prediction results require peak cases by county to be determined. 
   - Labels of "High", "Medium" and "Low" risk are then assigned to each county based on timeframe of when the peak value occurred 
2. Run cases.Rmd file to generate prediction model results and csv for case predictions by county
3. Run deaths.Rmd file to generate prediction model results and csv for deaths predictions by county
4. RStudio
5. Libraries
   - library(tidyr)
   - library(dplyr)
   - library(stringr)
   - library(ggplot2)
   - library(readr)
   - library(zoo)
   - library(scales)
   - library(sf)
   - library(urbnmapr)
   - library(plotly)
   - library(tidyverse)
   - library(mlbench)
   - library(caret)
   - library(stringr)

