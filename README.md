# Spatial-Analysis-Real-Estate-Development-Company
Analysis question: Should the development company build a small mixed-use development in the municipality of Gresham?

## Introduction ##
I'm acting a market analyst for a local development company. The company is currently trying to find out the optimal sites where can build small mixed-use developments.
The local company wants to build in a city that has large amount of land already zoned for mixed-use development, and also the company targets on people in their 20s and 
30s for both the retail and the rental purpose. 

## Ask Questions ##
In the case study, I'm going to determine key information about the city:
1. How much area is zoned for mixed-use development?
2. Where are high rental areas?
3. Where do high numbers of people between the ages of 22-39 live in high rental areas?

## Analyze and Explore data ##
Step 1: Filter data to limit feature display.
The first step is to filter the Gresham Zoning layer to display only the areas zoned for mixed-use development on the map.
I used `OR logical` to find area that meet the filter creteria: **Both Office Mix-use Residential (MUC1) and Downtown Mix-use Residential (MUC2)**
Check the below map, and these areas are symbolized with pink or maroon
![MUC1 and MUC2](https://github.com/mingyuan9/Spatial-Analysis-Real-Estate-Development-Company/blob/main/1.FilterMixUse.png)

Step 2: Examine statistics
In this step, I'm going to answer **How much area is zoned for mixed-use development?**
I used `Information` in the feature table and found out that slightly over 517 acres meet the criteria in either MUC1 or MUC2.
![information]()
