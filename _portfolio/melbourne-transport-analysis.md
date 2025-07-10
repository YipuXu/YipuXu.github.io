---
title: "Melbourne Public Transport Accessibility Analysis"
excerpt: "Urban Computing project analyzing Melbourne's public transport network accessibility and efficiency using GIS and data science techniques."
layout: custom
header:
  image: /images/portfolio-melbourne-transport.jpg
  teaser: /images/portfolio-melbourne-transport.jpg
order: 1
collection: portfolio
author_profile: true
---

# Report on Public Transport Accessibility in the Box Hill Area
*A University Project Prepared for Public Transport Victoria (PTV)*

## Project Overview

This project provides a comprehensive analysis of public transport accessibility and efficiency in the Box Hill area of Melbourne, conducted as a formal report for Public Transport Victoria (PTV). The core research question investigated how accessibility, stop coverage, passenger flow, and service frequency vary across Box Hill during peak hours to evaluate the network's efficiency and reliability. By integrating official PTV transport data with Australian Bureau of Statistics (ABS) geographical data, the project uses spatial-temporal analysis to identify service gaps and deliver data-driven recommendations for network improvement.

## 🎯 Objectives

- **Analyze Stop Coverage**: Determine which residential "mesh blocks" in Box Hill lack adequate transport coverage, defined as being more than 300 meters from a stop
- **Develop Accessibility Scores**: Calculate a quantitative accessibility score for each transport stop based on the number of routes it serves and its service frequency
- **Evaluate Peak-Hour Efficiency**: Assess service times, passenger flow, and average waiting times during peak commuting hours (7:00 AM - 9:00 AM) to identify bottlenecks
- **Provide Actionable Recommendations**: Use the findings to propose specific improvements for transport planning in the Box Hill area

## 🔧 Data & Methodology

### Datasets
- **PTV GTFS Dataset**: Utilized the version from March 17, 2023, containing detailed routes, schedules, and stop information for Melbourne's public transport network
- **ABS Geographical Data**: Employed Australian Statistical Geography Standard (ASGS) boundary data, specifically Mesh Blocks, the smallest unit for spatial analysis

### Methodology
- **Data Restoration & Preprocessing**: Established a `ptv` schema and created tables using SQL. Imported GTFS data using SQL `COPY` commands and performed extensive data cleaning, including filtering for the Melbourne boundary, linking stops to routes, and handling data conflicts to ensure integrity
- **Spatial Analysis**: Conducted detailed spatial analysis to identify unserved mesh blocks and analyze geographic patterns of service

### Key Technologies
- **Database**: PostgreSQL with PostGIS for spatial queries and data management
- **GIS Tools**: **QGIS** for creating heatmaps and other spatial visualizations
- **Programming**: **Python** for data processing and generating bar charts; **SQL** for all data restoration, preprocessing, and querying
- **Analysis Tools**: **Excel** for creating line charts

## 📊 Key Findings

### Accessibility Disparity
- A significant gap exists between the most and least accessible stops. **Box Hill Railway Station** is the most accessible with a score of **2,377**, while **Watts St/Whitehorse Rd** is the least accessible, scoring just **28**
- Several residential mesh blocks in Box Hill are more than **300 meters** from the nearest transport stop, indicating service gaps

{% include base_path %}

<figure class="image-map">
  <img src="{{ base_path }}/images/box-hill-underserved-areas.png" alt="Box Hill Underserved Areas Map">
  <figcaption>Map showing underserved residential areas (purple blocks) in Box Hill that are more than 300 meters from the nearest public transport stop. The analysis reveals significant service gaps in outer residential zones.</figcaption>
</figure>

### Service Imbalance & Peak Hour Pressures

#### Transport Mode Distribution
The Box Hill network shows a significant imbalance in transport mode coverage:

<figure class="image-chart">
  <img src="{{ base_path }}/images/box-hill-transport-pie-chart.png" alt="Public Transport Route Analysis for Box Hill">
  <figcaption>Distribution of public transport modes in Box Hill area. The overwhelming reliance on bus services (140 stops) compared to minimal tram (4 stops) and train (1 stop) coverage highlights the need for network diversification.</figcaption>
</figure>

- The Box Hill network is heavily reliant on **buses (140 stops)**, with minimal coverage from **trams (4 stops)** and **trains (1 stop)**

#### Peak Hour Analysis
Passenger traffic analysis reveals distinct peak periods and bottlenecks:

<figure class="image-chart">
  <img src="{{ base_path }}/images/hourly-arrival-departure-counts.png" alt="Hourly Passenger Flow Analysis">
  <figcaption>Hourly passenger arrival and departure counts throughout the day. The graph clearly shows peak periods during morning (8-9 AM) and evening (5-6 PM) commute times, with the highest activity at 5 PM (5,671 passengers).</figcaption>
</figure>

- Passenger traffic peaks between **8-9 AM and 5-6 PM**, with the highest count of **5,671 passengers at 5 PM**

#### Waiting Time Analysis
Peak hour service efficiency varies significantly across the network:

<figure class="image-map">
  <img src="{{ base_path }}/images/box-hill-waiting-times-heatmap.png" alt="Peak Hour Waiting Times Heatmap">
  <figcaption>Heatmap visualization of average waiting times during peak hours. Red areas indicate longer waiting times, with Surrey Park/Canterbury Rd showing the highest delays. This spatial analysis helps identify priority areas for service improvement.</figcaption>
</figure>

- During morning peak hours, some stops experience long delays, with **Surrey Park/Canterbury Rd** having the longest average wait time of **12 minutes and 37.5 seconds**

## 🚀 Impact & Recommendations

### Targeted Improvements
- The analysis identified specific areas needing upgrades, such as the low-accessibility Watts St/Whitehorse Rd area and high-wait stops like Surrey Park

### Network Diversification
- Findings suggest that expanding the limited tram and train services could create a more balanced and robust transport network in Box Hill

### Stakeholder Engagement
- The final report and its data-driven recommendations were prepared for **Public Transport Victoria (PTV)**, providing valuable insights to inform their future transport planning

## 🎨 Visualizations

The report featured a range of visualizations to clearly communicate findings:

- **Heatmaps in QGIS** to highlight areas with long waiting times and missing stop coverage
- Geographic maps showing stop density and peak-hour passenger counts
- **Python-generated bar charts** to depict service durations for different stops
- **Excel-generated line charts** to illustrate hourly passenger arrival and departure counts

## 📈 Technical Skills Demonstrated

- **End-to-End Data Analysis**: From raw data restoration and SQL preprocessing to complex spatial analysis and final reporting
- **Spatial Data Management**: Proficient use of PostgreSQL/PostGIS for handling and querying geographic data
- **Multi-Tool Proficiency**: Combined the strengths of SQL, Python, QGIS, and Excel to conduct a comprehensive analysis
- **Stakeholder Communication**: Translated complex technical findings into clear, actionable insights for a public-sector client (PTV)

## 🔮 Future Enhancements

The project identified several areas for future work based on its limitations:

- Incorporate more granular passenger movement data for higher accuracy
- Address potential data quality issues, such as incomplete passenger counts for some stops
- Expand the analysis scope with more time to cross-reference other datasets for more robust results

---

*This project demonstrates the application of urban computing and spatial data science techniques to solve real-world transportation challenges, showcasing the integration of multiple data sources and analytical tools to provide actionable insights for public policy and infrastructure planning.* 