# King County, Washington House Sales – Tableau Dashboard


![King County, Washington House Sales Dashboard](https://github.com/maryamsh62/Tableau-Portfolio-Project---King-County-Washington-House-Sales/blob/master/King%20County%20Dashboard.png)

[TableauPublic](https://public.tableau.com/app/profile/maryamsadat.shakeri/viz/KingCountyWashingtonHouseSales_17612712919360/Dashboard1)


## Project Overview

This repository contains a Tableau project that analyzes residential house sales in King County, Washington.
The main goal is to let users explore how house prices vary over time, by location, and by property characteristics through an interactive dashboard.


**The goal of this project is:** 

- How do daily average sale prices change within a given month?
- Which neighborhoods/areas in King County have higher average prices?
- What is the distribution of sale prices, and where is the bulk of the market?
- How do the number of bedrooms and bathrooms typically distribute across sold homes?
- How do view and condition together affect the average selling price?



## Project Files

- `King County, Washington House Sales.twbx`: Packaged Tableau workbook containing the finished dashboard.
- `HouseData.xlsx`: Source dataset used by the workbook.
- `King County Dashboard.png`: The picture of the main dashboard.



## Dataset

The dataset includes individual house sale records for King County, WA.

**Key fields used in the dashboard include:**

- **date** – date of sale (used as the primary time filter)
- **price** – sale price
- **bedrooms, bathrooms**
- **sqft_living, sqft_lot**
- **yr_built**
- **view, condition**
- **lat, long, or geographic fields such as zipcode/neighborhood**

**Important data step:**

- In Tableau, change the data type of the date column to Date (not string or date-time) so the calendar filter and time-series chart work correctly.



## Dashboard Overview

The dashboard is built around a calendar widget as the main filter, and includes several supporting views:

1. Filter Panel 

   - `Month dropdown + calendar:`
     Select a month from the dropdown and a specific day from the calendar to filter all views on the dashboard.

   - `Year Built slider:`
     Filter properties by construction year.

   - `Sqft Living slider:`
     Restrict results by interior living area.

   - `Sqft Lot slider:`
     Restrict results by lot size.

   These filters are global and update every chart and the map simultaneously. 
   

2. Daily Average House Sales Price 

   A line chart of average sale price by day for the selected month, revealing short-term trends and daily price volatility.


3. Map – Spatial Distribution 

    - Filled map of King County, Washington.

    - Geographic areas are colored by average sale price (or a related measure), allowing quick comparison across locations.  
   

4. Distribution of House Prices (Middle-Left)

   A histogram of sales frequency by price bin helps identify the most common price ranges and reveal any market skewness. 
   

5. View vs. Condition Heatmap 

   - Rows represent property view categories 

   - Columns represent condition categories 

   Each cell displays the average sale price for that combination, highlighting how physical condition and view quality interact to influence price.
   

6. Distribution of Bedrooms (Bottom-Left)

   A histogram of bedroom counts shows how houses are typically sized by number of bedrooms, highlighting the most common configurations (3–4 bedrooms).
   
   
7. Distribution of Bathrooms 

   A histogram of bathroom counts complements the bedroom distribution by describing typical home layouts in terms of the number of bathrooms.



## Results

- The daily average house sale price for the selected period (e.g., June 2014) remains within a relatively stable range, with a few noticeable peaks that indicate short-term volatility but no extreme swings in the local market during that month.

- The price distribution is right-skewed: most homes sell within a mid-range band, while a smaller number of high-end properties extend the upper tail of the distribution.

- Three- to four-bedroom homes represent the majority of sales, with two to three bathrooms being the most common, indicating that typical King County buyers are targeting standard family-sized homes.

- The map shows clear geographic price differences: areas closer to Seattle and/or waterfront locations tend to have higher average prices, while some outlying regions remain more affordable.

- The View vs. Condition heatmap highlights a strong relationship between property quality and price: Homes in Good/Very Good condition with Average to Excellent view achieve the highest average prices.

- Properties with poor condition and no view cluster are at the lower end of the price spectrum. 

- Filters for year built, square feet of living space, and lot size reveal that newer, larger homes generally command higher prices, although this effect is moderated by location, view, and overall condition. 



## Conclusion

The dashboard shows that King County house prices are primarily driven by location, property condition, and home size.
Most demand centers on family-oriented homes with 3–4 bedrooms and 2–3 bathrooms, where larger and newer properties generally sell for more.
Buyers, sellers, and real-estate professionals can use the dashboard to see what drives price differences and which upgrades (e.g., condition, curb appeal, views) offer the best returns. 


`License`

Feel free to adapt and extend this project for learning and portfolio purposes.

