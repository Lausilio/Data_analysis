# Analysis of Vodafone Users' Fluxes in Padova

This repository houses a comprehensive project that analyzes the flux of people inside urban areas, with a focus on the city of Padova, Italy. The project aims to understand critical issues in local mobility and explore areas of potential improvements in the infrastructure and local transports. 

## Project Overview

The project uses data provided by the Vodafone mobile carrier, which monitors the mobility of users within and toward Padova based on users' connections to network cells. The data was collected over a four-month period from February to May of 2018 and is provided in .csv files. Privacy is protected by aggregating data and discarding observations with less than 30 units.

## Datasets

The data includes the following .csv files:

- `day_od.csv`: Contains details about users' origins and destinations, averaged by the day of the week. 

- `distinct_users_day.csv`: Contains details about the number of distinct users by origin.

Three lookup tables are also provided to match the ISTAT country, province, and comune codes to their actual names:

- `codici_istat_comune.csv`
- `codici_istat_provincia.csv`
- `codici_nazioni.csv`

Additional information such as the number of inhabitants of each province and the distance between Padova and all other Italian provinces can be extracted from the data collected by ISTAT.

## Assignment

The project involves the following tasks:

1. Data preparation: Ensuring each .csv file is properly interpreted.
2. Ranking of visitors from foreign countries: Creating a ranked plot of the first 20 countries with the most visitors.
3. Ranking of Italian visitors by province, weighted by the number of inhabitants: Creating a ranked plot of the first 20 provinces with the most visitors, taking into account the number of inhabitants.
4. Study of the visitors' fluxes: Analyzing the three main directions of visitors and commuters getting to Padova by the Italian highways (south: A13 toward Bologna-Roma / west: A4 toward Milano-Torino / north-east: A4 toward Venice-Trieste) to determine which direction should be prioritized for investment in mobility improvements.
   - Consider a simplified case involving only mid-range mobility, based on the number of visitors/commuters from nearby regions only.
   - Consider the provinces located on the three directions that mostly contribute to the flow of weekend visitors and working daily commuters by performing a detailed study of the fluxes based on the day of the week.
   - Use the data available to provide the best possible answer.
5. Plot the distribution of the number of visitors by the distance of the province of origin, and determine which kind of law should be used to describe the distribution.
6. Create a regression to estimate the expected number of visitors by the distance of the province of origin. Illustrate the difference between the resulting regression and the numbers provided by the Vodafone monitoring, and highlight the five most striking discrepancies from the expectations.
7. Extract additional interesting information concerning mobility and the flux of visitors and commuters using all the data available (and additional data from ISTAT sources if needed).
