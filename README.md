# Global Energy Trade Analysis

## Project Description

This project provides a comprehensive analysis of global energy trade patterns from 1990 to 2020. Using datasets covering energy imports, exports, and production, this analysis aims to visualize and uncover key trends, identify major players in the energy market, and explore the changing dynamics of the global energy landscape over the last three decades.

Interactive dashboards have been developed in both **Power BI** and **Tableau** to allow for dynamic exploration of the data.

## Tools Used

* **Data Transformation:**
    * Power Query
* **Data Analysis & Visualization:**
    * Microsoft Power BI
    * Tableau

## Data Source

The core dataset was sourced from Kaggle:
* **Kaggle Dataset:** [Energy Data 1990-2020](https://www.kaggle.com/datasets/shub218/energy-data-1990-2020)
* **Original Source:** The dataset is a compilation from the [UN Energy Statistics Yearbook](https://unstats.un.org/unsd/energystats/pubs/yearbook).

## Project Files & Data Model

This project uses a simple star schema model, optimized for analysis in Power BI and Tableau.

* `Global Energy Trade Data.csv`: This is the primary **fact table**. It contains the cleaned and transformed transactional data, including energy imports, exports, and production values by country, year, and energy type.
* `DateTable.csv`: This is a **dimension table** connected to the main fact table. It contains date-related attributes (e.g., Year, Decade) to enable robust time-based analysis and filtering.
* `MeasureTable.csv`: This table was used primarily in the Power BI model to logically group and organize **DAX measures** (e.g., Total Imports, Total Exports, Year-over-Year Growth), improving model organization and usability.

## Key Analyses & Visualizations

The dashboards in this project are designed to answer questions such as:

* What are the overall trends in energy production, imports, and exports from 1990 to 2020?
* Who are the top energy-producing, importing, and exporting countries?
* How has the energy mix (e.g., fossil fuels vs. renewables) evolved over time for specific countries or globally?
* What are the geographical patterns of energy trade (visualized using maps)?
* How does energy balance (Production vs. Consumption) vary by country and over time?

## How to Use

### Power BI

1.  Ensure you have **Power BI Desktop** installed.
2.  Open the file: `Global Energy Trade Analysis.pbix`
3.  Interact with the slicers, filters, and visuals to explore the data.

### Tableau

1.  Ensure you have **Tableau Desktop** or **Tableau Reader** installed.
2.  Open the file: `Global Energy Trade Analysis.tbw`
    * **Important Note:** A `.tbw` file (Tableau Workbook) only contains the dashboard structure and links to the data sources. Anyone opening this file will need to download the `.csv` files separately and re-connect the data source.
    * **Suggestion:** For easier sharing, consider saving your Tableau file as a `.twbx` (Tableau Packaged Workbook) instead. This bundles the data files directly into the Tableau file.
3.  Use the filters and dashboard actions to navigate and analyze the visualizations.
