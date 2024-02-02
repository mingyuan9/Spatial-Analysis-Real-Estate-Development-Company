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
**Step 1: Filter data to limit feature display**
The first step is to filter the Gresham Zoning layer to display only the areas zoned for mixed-use development on the map.
I used `OR logical` to find area that meet the filter creteria: **Both Office Mix-use Residential (MUC1) and Downtown Mix-use Residential (MUC2)**
Check the below map, and these areas are symbolized with pink or maroon.

![MUC1 and MUC2](https://github.com/mingyuan9/Spatial-Analysis-Real-Estate-Development-Company/blob/main/1.FilterMixUse.png)

**Step 2: Examine statistics**
In this step, I'm going to answer **How much area is zoned for mixed-use development?**
I used `Information` in the feature table and found out that slightly over 517 acres meet the criteria in either MUC1 or MUC2.

![information](https://github.com/mingyuan9/Spatial-Analysis-Real-Estate-Development-Company/blob/main/2.statistics.png)

**Step 3: Enrich Block Group layer by adding attribute information**
I applied `Analysis` in the Setting toolbar and by adding `enrichment variables` in the Block Group, I successfully added `2023 Renter Occupied HUs` attibute in the layer.

![Addting attribute to layer](https://github.com/mingyuan9/Spatial-Analysis-Real-Estate-Development-Company/blob/main/3.AddingAttribute%20toLayer.png)

**Step 4: Calculate field**
The development company also wants to determine how many young people btween 20s and 30s reside within these block groups.
Since the data was seperated in two columns `AGE_22_29` and `AGE_30_39`, I need to sum the number together by adding a new column `AGE_22_39` to this attribute table.

![addting new column to attribute table]()

## Analyze and Model ##
**Apply labels**
In order to make the map more informative, I decided to apply labels to the Enriched Block Group Renters layer. 
It's now easily to view the population of people between the age of 22-39 for each block group.

![AddingLabels]()

**Analysis by Visualization**
From information of 2023 Renter Occupied HUs field in attribute table, we've seen that the block groups have an average over 394 number of rental units.
Then, I added an `expression` in `Style` to get a more effective visualization of rental housing.
This graph also explains question that **Where do renters live within the city?**
You can find that most rentals are found in block groups closer to the city center in Gresham or northwest of the city center.

![RENTER_CY > 394]()
