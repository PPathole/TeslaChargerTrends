# TeslaChargerTrends

# Tesla Supercharger Insights

This repository contains a comprehensive analysis of Tesla Supercharger data, focusing on exploring and visualizing key insights using both Python (for preprocessing) and Excel (for analysis). The dataset includes information about various Supercharger stations around the world, with columns for Supercharger name, address, city, state, zip code, country, number of stalls, power output (kW), GPS coordinates, elevation, and open date.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
  - [Handling Date Column](#handling-date-column)
  - [Standardizing Zip Column](#standardizing-zip-column)
  - [Standardizing State/Region Names](#standardizing-state-region-names)
- [Excel Analysis](#excel-analysis)
  - [Descriptive Statistics](#descriptive-statistics)
  - [Pivot Tables](#pivot-tables)
  - [Visualizations](#visualizations)
  - [Advanced Analysis Questions](#advanced-analysis-questions)
- [Getting Started](#getting-started)
- [Contributing](#contributing)

## Introduction

This project aims to uncover meaningful insights from Tesla Supercharger data through comprehensive data preprocessing and analysis. The analysis is conducted using Excel, leveraging its powerful data manipulation and visualization capabilities.

## Dataset

The dataset contains the following columns:

- `Supercharger`: Name of the Supercharger station
- `Street Address`: Address of the station
- `City`: City where the station is located
- `State`: State or region
- `Zip`: Zip code
- `Country`: Country where the station is located
- `Stalls`: Number of charging stalls at the station
- `kW`: Power output of the station
- `GPS`: GPS coordinates
- `Elev(m)`: Elevation of the station in meters
- `Open Date`: Date when the station was opened

## Preprocessing

### Handling Date Column

The `Open Date` column contained null values and dates in different formats. The preprocessing steps involved:

- Parsing dates in various formats to a standard format.
- Filling null values with a placeholder date (e.g., `1970-01-01`).

### Standardizing Zip Column

The `Zip` column was standardized to ensure consistency:

- Handling leading zeros and ensuring zip codes are in a string format.
- Filling null values with a placeholder (e.g., `00000`).

### Standardizing State/Region Names

State and region names were standardized across multiple countries. A mapping function was created to convert full state names to their abbreviations or standardized forms for various countries (e.g., USA, Canada, Australia).

## Excel Analysis

### Descriptive Statistics

Using Excel's `Data Analysis` tool, we computed descriptive statistics (mean, median, mode, standard deviation) for columns like `Stalls` and `kW`.

### Pivot Tables

Several pivot tables were created to summarize data:

- **Total Number of Stalls per Country**: Summarized the total number of stalls in each country.
- **Average kW per Country**: Calculated the average power output per country.
- **Number of Superchargers per State/Province**: Counted the number of Supercharger stations in each state/province.

### Visualizations

We created various charts to visualize the data:

- **Bar Chart for Total Stalls per Country**: Displayed the total number of stalls in each country.
- **Line Chart for kW Trends**: Showed the average power output over time.

![KWh Trend](https://github.com/PPathole/TeslaChargerTrends/blob/main/Screenshot%202024-07-12%20at%2021.32.36.png)

- **Pie Chart for Distribution of Superchargers by Country**: Illustrated the proportion of Supercharger stations in each country.
- **Heatmap for Stalls and kW**: Visualized the density of stalls and power output across different states and cities.

### Advanced Analysis Questions

1. **Distribution of Supercharger Stations Across Different Countries**:
   - Counted the number of Supercharger stations per country and visualized it using a pie chart.

2. **States/Provinces with the Highest Number of Supercharger Stalls**:
   - Summarized the total stalls by state/province within each country using a bar chart.

3. **Average Power Output (kW) by Country and State/Province**:
   - Compared the average power output by country and state/province using a clustered column chart.

4. **Trends in Number of Superchargers Installed Over Time**:
   - Analyzed the growth trend of Superchargers installed over time with a line chart.

  ![Maps](https://github.com/PPathole/TeslaChargerTrends/blob/main/Screenshot%202024-07-14%20at%2014.58.21.png)

5. **Relationship Between Number of Stalls and kW Capacity**:
   - Created a scatter plot to explore the correlation between the number of stalls and power output.

6. **Effect of Elevation on Stalls and kW**:
   - Examined how elevation affects the number of stalls and power output using line charts and bar charts.
  
![Supercharger Analysis](https://github.com/PPathole/TeslaChargerTrends/blob/main/Screenshot%202024-07-12%20at%2021.32.09.png)

![Gaps](https://github.com/PPathole/TeslaChargerTrends/blob/main/Screenshot%202024-07-14%20at%2014.56.58.png)

## Getting Started

To get started with the analysis:

1. Clone the repository:
   ```sh
   https://github.com/PPathole/TeslaChargerTrends
   ```
2. Open the Excel workbook `tesla_superchargers.xlsx` to explore the analysis.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please submit a pull request or open an issue.
