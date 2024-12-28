# Lego-report-powerbi
Power BI report analyzing over 4,000 LEGO sets based on pieces, price, and age range

**LEGO Report Using Power BI
Project Overview**
This project explores the world of LEGO sets through a detailed analysis of over 4,000 LEGO sets, dating back to 1970. The aim was to assist an avid LEGO collector in identifying the perfect next set by analyzing key features such as the number of pieces, age range, and price. The dataset was provided in CSV format and imported into Power BI for data preparation, analysis, and visualization.

**Data Preparation and Cleaning**
Data preparation was carried out using Power Query in Power BI, focusing on the following steps:

**Column Removal:** Excluded unnecessary fields like minifigs, bricksets_url, and thumbnail.

**Data Profiling:**
Verified the accuracy of header names and data types.
Filtered out records missing crucial fields like price, age, number of pieces, and image_url.
**Feature Engineering:** Created new conditional columns for better categorization:
**Age Range**: Categorized into 1-4, 5-9, 10-17, and 18+.

**Price Range:**
$ for <$25
$$ for $25 - $49.99
$$$ for $50 - $99.99
$$$$ for $100 - $499.99
$$$$$ for ≥$500.

**DAX Measures and Parameters**
Several DAX measures were implemented for deeper insights:

Total Sets: DISTINCTCOUNT(lego_sets[set_id])
Total Theme Groups: DISTINCTCOUNT(lego_sets[theme_group])
Average Price: AVERAGE(lego_sets[price])
Average Pieces: AVERAGE(lego_sets[pieces])
Average Age: AVERAGE(lego_sets[age])
A parameter was also created to allow dynamic filtering based on price.

**Visualizations**
The Power BI report features interactive visuals, including:

**Total Metrics**: Displaying the total number of LEGO sets, average pieces per set, and average price.

**Filters**: Enabling users to explore LEGO sets by:
Theme Group
Theme
Age Range
Price Range
Highlights:
Distribution of LEGO sets by price, age, and theme.
Analysis of specific LEGO themes like "Star Wars" and "Ninjago."

Insights
**Key insights from the report include**:

The collection includes 4,385 unique LEGO sets.
The average number of pieces per set is 411.
The average price across all sets is $45.
Dynamic filters make it easy to identify sets that match specific criteria.
Tools Used
Power BI Desktop: For data preparation, analysis, and visualization.
Power Query: For data cleaning and transformation.
DAX (Data Analysis Expressions): For custom calculations.

![Dashboard Overview](path-to-your-screenshot.png)

