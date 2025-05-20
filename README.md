# Video Games Sales Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
-  [Recommendations](#recommendations)
-   [References](#references)

### Project Overview
Nexatel, a hypothetical company aspiring to enter the video game market, leverages historical data from various regions, including Europe, North America, Japan, and others. The company aims to analyze what has worked and what has not over time. Key metrics for analysis include genre, platforms, publishers, global sales, and trends. The insights are aimed at helping the company decide whether to venture into the video game business.

![For_Github](https://github.com/user-attachments/assets/43229ddd-e6ca-4b68-ac17-02416da64a62)




### Data Sources
Blossom Academy Sales Data: The primary dataset used for this analysis is "vgsales.xlsx" file.

### Tools
-  Power BI: Data Cleaning, Data Analysis, Data Visualization
    -   [Download Power BI here](https//microsoft.com)

### Data Preparation
I completed the following key steps:
-  Loaded data into Power Query 
-  Cleaned and formatted the data
    -   promoted headers, changed data type, replaced values, filed down

### Exploratory Data Analysis
This involves examining the sales data to address key questions, including:
- What are top-selling video games globally and regionally?
- What are the most popular genres, platforms, and publishers?
- What are the sales trends over the years?
- When are the peak sales?

### Data Analysis
The data analysis involved for this project featured the following DAX:
-	Creating of parameter:
  
```Sales category = {("Europe", NAMEOF('vgsales'[Sum_eu_sales]), 0),("Global", NAMEOF('vgsales'[Sum_global_sales]), 1),("Japan", NAMEOF('vgsales'[Sum_jp_sales]), 2),("N. America", NAMEOF('vgsales'[Sum_na_sales]), 3),("Others", NAMEOF('vgsales'[Sum_other_sales]), 4)}```

-	Using ```SUM``` and ```AVERAGE``` functions:
  
 ```Sum_global_sales = SUM(vgsales[Global_Sales])```
 
```Sum_eu_sales = SUM(vgsales[EU_Sales]) ```

```Sum_jp_sales = SUM(vgsales[JP_Sales]) ```

```Sum_na_sales = SUM(vgsales[NA_Sales]) ```

```Sum_other_sales = SUM(vgsales[Other_Sales]) ```


```Avg. Global Sales = AVERAGE(vgsales[Global_Sales])```

```Avg. Sales Europe = AVERAGE(vgsales[EU_Sales]) ```

```Avg. Sales Japan = AVERAGE(vgsales[JP_Sales]) ```

```Avg. Sales NA = AVERAGE(vgsales[NA_Sales]) ```

```Avg. Sales other = AVERAGE(vgsales[Other_Sales]) ```

    
### Results and Findings
The analysis results are summarized as follows:
-  Top Games and Regions
Wii Sports topped the global charts, followed by Grand Theft Auto V and Super Mario Bros, similarly North America and Europe emerged as the key regions for the gaming business.
-  Popular Genres:
Action and Sports were the most beloved genres across the regions studied.
-  Leading Publishers:
Nintendo leads the market in global sales, followed by Electronic Arts and Activision.
Nintendo published 7 of the top 10 bestsellers, including Wii Sports.
-  Platform Preferences:
Besides the Wii and DS, the PS2 platform is a favorite among top publishers.
-  Sales Trends:
The gaming industry reached its peak sales between 2006 and 2008, followed by a steady decline from 2009 to 2017. Contributing factors included the shift to mobile gaming, technological advancements, poor game quality, marketing issues, and changing consumer preferences.

### Recommendations
From the insights derived, the following actions are recommended:
- Develop high-quality games for handheld platforms like phones and PCs to capture the current market trends.
- Invest in popular genres (Action, Sports) and platforms (PC, PS4) to maximize sales potential.
### References
- Data Analysis with Power BI on DataCamp
   -    [DataCamp](https//Datacamp.com)


