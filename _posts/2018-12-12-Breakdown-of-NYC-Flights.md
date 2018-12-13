---
title: Analysis of NYC Flights in the year 2013
---
# Final Project - Introduction to Big Data Visualization

## In this project I am to gain a better understandting of flights from New York City's major airports, Laguardia, JFK and Newark for the year 2013. I discovered many insteresting facts in regards to departure flights and their destination. The numbers show that Newark airport handles more flights and JFK the least but JFK Air routes cover the most amount of Air miles than the other airports. we discovered that the airports most travelled to by NYC passengers are Charlotte, Atlanta and Raleigh-Durham. These are all known HUBS for airlines. The data supports that most airlines are now using airports as hubs to make connections in an effor to maximize the amounts of seats are filled. I also wanted to look at the effeciency of each carrier and found Expressjet to have the highest positive ratio in the industry and the least efficient Alaskan Air. below is the complete analysis, project workflow, limitations and Tableu workbook with supporting visualizations. 

# Analysis of NYC flights

## A statistical breakdown of flights arriving and departing from the Greater New York City major airports. LaGuardia (LGA), JFK and Newark (EWR). The dataset collected flight information from the 3 major airports for the year of 2013. With all the information collected I will be able to create a breakdown of several different factors that will help me breakdown flight information. For my story I used many different data fields. Origin tags outbound aircraft and which airport they depart from. Sum of distance is the accumulation of all flight miles. Sum of flights is the accumulation of all flights includes departure and arrivals. Dest shows all the airport codes which the airports have travelled to. Carrier is all the airlines that have operated in the airports Tableau is a visualization tool that allows you to create easy to understand visuals from a busy and complex dataset from excel. Tableau allows you to compare different datasets easily and manipulate visuals easier than excel. 

# Project Workflow

## Downloaded the dataset from https://data.world/bob-wakefield/flights and imported to Tableu as other. Once successfully imported I created a multiple calculated field First Dep Delay:  IF [Dep Delay] < 0 THEN NULL ELSE [Dep Delay] END. With the purpose to remove all the times when an airline left early so no positive values will change the efficiency table. I wanted to only look at the negative numbers which meant the tardy efficiency of each airline would only look at late flights and not consider those that left early. Second Avg(Delays to Flight ratio) is [Flight] / [Dep Delay] which creates a positive ratio for efficiency the higher the number the more efficient that dimension is. Third Placeholders are set up to create Labels for Text Tables. 

## On the visual Destination by flights I created a parameter for Number of flights, so the user can adjust the number and have a clear visual of the routes that were flown above and below whatever your target may be. This also allows you to concentrate on the top routes our of NYC airports.

## Filters used under Most Flight Destination dashboard I used Carrier, Dest and Origin. This allows a user to tinker and center in on a specific route, airline or airport. On the text table I added the filters Dest and Origin. For user to simplify the list.

## Tooltips used in distance travel by airport include Origin, Sum(Distance) and Sum(hour) this allows the user to quickly see the amount of flight miles and hours that each airport was involved in. in Airport by flights I used Origin and amount of flights so the user can see amount of flights without looking at the graph on the left. Destination by flights include Dest to easily see which route your on, Avg delays to ratio so you can see the effectiveness of the route and flights, so you can see the actual amount of flights in that flight route. Carrier by AVG departure delay I used the tooltips carrier, avg delays to flights ratio and flight.

# Limitations

## The downside of the dataset is that it did not include where all the flights were coming from. This prevented me a comparison of departure destinations and arrival destination. Would have also liked to have had the coordiantes of each Destination and Origin to create a geographical visual.

# Tableu Workbook

<iframe src = "https://public.tableau.com/views/AnalysisofNYCFlights/MostEffecientAirline?:embed=y&:display_count=yes" width="800" height="655"></iframe>
