# Philippine Emigrants Tableau Dashboard

# Table of Contents
* [Project Background](#project-background)
* [Data Structure and Initial Checks](#data-structure-and-initial-checks)
* [Executive Summary](#executive-summary)
* [Insights Deep Dive](#insights-deep-dive)
* [Recommendations](#recommendations)
* [Assumptions and Caveats](#assumptions-and-caveats)
* [Credits and Acknowledgements](#credits-and-acknowledgements)

---

# Project Background
The Philippines has one of the highest emigration rates in the world, and is among the highest in Southeast Asia ([see this repo for more details](https://github.com/Francis-Calingo/Socioeconomic-Analysis-of-The-Philippines)). In Canada, emigrants leaving the Philippines are one of the top sources of immigration ([see this repo for more details](https://github.com/Francis-Calingo/Visualizing-Migration-in-Canada?tab=readme-ov-file#time-series-analysis)), and is rapidly growing in certain regions ([see this repo for more details](https://github.com/Francis-Calingo/ELECTIONS-CANADA-RESEARCH-PROJECT-Filipino-Canadian-Demographic-Report)). Using data from the Commission of Overseas Filipinos' Registered Emigrants datasets, this Tableau dashboard visualizes emigration from the Philippines in the following areas:

- **Time-Series Progression of Migration**
- **International Destinations** 
- **Place of Origin** 

The interactive Tableau dashboard used to report and explore this topic can be found [here](https://public.tableau.com/app/profile/francis.emmanuel.calingo/viz/DataonRegisteredFilipinoEmigrantsSincethe1980s/NumberofRegisteredFilipinoEmigrantsSince1981).

To download the Tableau workbook version, [click here](https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/raw/main/Filipino%20Emigration%20Trends%20(1981–Present).twbx)

<i>Preview of Dashboard:</i>

<img src=https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/blob/main/Figures/Dashboard.png/>

**Tools and Technologies Used:**

* **Visualization Platform:** Tableau Public

* **Data Wrangling:** Excel (cleaning, reshaping)

* **Interactivity Features:** Hover tooltips, Navigation buttons


Data Sources: [Dataset names or links]


[<b>Back to Table of Contents</b>](#table-of-contents)

---

# Data Structure and Initial Checks

The data structure for the data utilized to build this dashboard is as follows:

| Data Content  | Number of Entries (Records x Field) | Number of Records  | Number of Fields | Download File Link |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Emigrant Data-All Country Destinations | **465**  | 155  | 3  | [Download](https://raw.githubusercontent.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/main/CSV%20Files/Emigrant-1981-2022-AllCountries.csv)  |
| Emigrant Data-Major Country Destinations  | **559**  | 43   | 13  | [Download](https://raw.githubusercontent.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/main/CSV%20Files/Emigrant-1981-2022-MajorCountry.csv) |
| Emigrant Data-Major Country Destinations (Total)  | **22**  | 11  | 2 | [Download](https://raw.githubusercontent.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/main/CSV%20Files/Emigrant-1981-2022-MajorCountry%20Total.csv) |
| Emigrant Data-Provincial Origins | **405**  | 81  | 5  | [Download](https://raw.githubusercontent.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/main/CSV%20Files/Emigrant-1981-2022-PlaceofOrigin%20Province.csv) |
| **TOTAL** | **1,451**  | 290  | 23  | N/A  |

**Calculations and Data Viz Development:**
* **Panel 1:** Number of Registered Filipino Emigrants Since 1981
  * Type: Bar and Line Dual-Axis Plot
  * Data: Emigrant-1981-2022-MajorCountry
  * Column: Year
  * Row (2): SUM(Total), SUM(Total)-Running sum

* **Panel 2:** Registered Filipino Emigrants by Destination Country, 1981-2022
  * Type: Vertical Bar Chart
  * Data: Emigrant-1981-2022-MajorCountry Total
  * Column: Country
  * Row: SUM(Total)
 
* **Panel 3:** Percentage of Registered Filipino Emigrants by Country of Destination, 1981-2022
  * Type: Choropleth Map
  * Data: Emigrant-1981-2022-AllCountries
  * Measure: SUM(% Total Emigrants)
  * Dimension: Country
  * Column: Longitude(generated)
  * Row: Latitude(generated)
 
* **Panel 4:** Total Registered Filipino Emigrants by Origin, 1988-2023 (per 100,000, 2020 PH Census)
  * Type: Choropleth Map
  * Data: Emigrant-1981-2022-PlaceofOrigin Province
  * Measure: SUM(Emigrants per Capita)
  * Dimensions: Country, Province
  * Column: Longitude(generated)
  * Row: Latitude(generated)


[Entity Relationship Diagram here]

[<b>Back to Table of Contents</b>](#table-of-contents)

---

# Executive Summary

### Overview of Findings

Explain the overarching findings, trends, and themes in 2-3 sentences here. This section should address the question: "If a stakeholder were to take away 3 main insights from your project, what are the most important things they should know?" You can put yourself in the shoes of a specific stakeholder - for example, a marketing manager or finance director - to think creatively about this section.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Time-Series Progression of Migration:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

<img src=https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/blob/main/Figures/Panel%201.JPG>



### International Destinations:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

<img src=https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/blob/main/Figures/Panel%202.JPG>

<img src=https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/blob/main/Figures/Panel%203.JPG>


### Place of Origin:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

<img src=https://github.com/Francis-Calingo/Philippine-Emigrants-Tableau-Dashboard/blob/main/Figures/Panel%204.JPG>

[<b>Back to Table of Contents</b>](#table-of-contents)

---

# Recommendations:

Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following: 

* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
[<b>Back to Table of Contents</b>](#table-of-contents)

---

# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)

[<b>Back to Table of Contents</b>](#table-of-contents)

---

# Credits and Acknowledgements

[<b>Back to Table of Contents</b>](#table-of-contents)
