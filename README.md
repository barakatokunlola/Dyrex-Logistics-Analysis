# Dyrex Logistics Analysis 

## Introduction
The Dyrex Logistics Analysis project explores the financial and operational performance of a logistics company using Microsoft Power BI. The project combines multiple datasets covering loads, customers, routes, trips, drivers, trucks, fuel purchases, delivery events, maintenance records, and safety incidents.

The objective is to transform raw operational data into meaningful insights that support business performance monitoring, revenue analysis, fleet management, delivery performance evaluation, maintenance planning, and safety monitoring. The analysis was developed using Microsoft Excel, Power Query, Power BI, and DAX and presented through a four-page interactive dashboard.

## Problem Statement
Logistics operations involve several interconnected activities, including customer management, shipment processing, revenue generation, transportation, fuel consumption, fleet utilization, vehicle maintenance, and delivery scheduling. Without a consolidated reporting solution, it can be difficult for management to monitor these activities, understand performance trends, identify operational risks, and make informed decisions.

Dyrex Logistics requires an integrated view of its financial and operational performance to understand revenue generation, evaluate fleet and driver activities, monitor delivery reliability, and assess maintenance and safety performance. This project addresses these needs by preparing and analyzing multiple logistics datasets and presenting the results through an interactive Power BI dashboard.

## Business Questions
### 1. Business Overview
 • What are the company’s overall revenue and operational activity levels?
 
 • How does revenue vary over time?
 
 • Which customers, routes, and truck makes contribute to business activity?
 
 • How many loads and trips are recorded?
 
 • What proportion of delivery events are completed on time?
 
 • How can financial and operational KPIs support management decisions?
 
### 2. Customers and Revenue
 • Which customers generate the highest revenue?
 
 • How is revenue distributed across customer types?
 
 • How do Dry Van and Refrigerated loads compare in volume and revenue?
 
 • How do booking arrangements contribute to revenue?
 
 • What additional charges and fuel surcharges are associated with loads?
 
 • Which customer segments may offer opportunities for improved revenue generation?
 
### 3. Drivers and Fleet
 • How many trips are recorded across the fleet?
 
 • How do driver revenue and operational performance vary?
 
 • How effectively are trucks being utilized?
 
 • What patterns exist in mileage and fuel efficiency?
 
 • How do fuel costs vary across drivers and fleet operations?
 
 • Which areas may require further investigation to improve fleet efficiency?
 
### 4. Maintenance and Safety
 • What are the total recorded maintenance costs and downtime?
 
 • Which maintenance categories account for the highest costs?
 
 • How does maintenance downtime change over time?
 
 • How many safety incidents have been recorded?
 
 • Which incident categories account for the most incidents and claims?
 
 • How can maintenance and safety data support better operational risk management?
 
## Data Source
The project uses a ZIP archive containing 14 CSV datasets, which was extracted into a document file.
The datasets cover the following areas:

**1. Loads:** shipment records, load dates, load types, customers, routes, revenue, fuel surcharges, additional charges, and load status.

**2. Customers:** customer information, customer types, account status, freight preferences, credit terms, and annual revenue potential.

**3.Trips:** trip records, assigned drivers and vehicles, dispatch dates, distance, duration, fuel consumption, and trip status.

**4. Drivers:** driver information, employment status, experience, license details, and home terminals.

**5. Trucks:** truck information, makes, model years, fuel types, acquisition details, and vehicle status.

**6. Trailers:** trailer inventory, trailer types, specifications, acquisition details, and status.

**7. Routes:** route origins and destinations, typical distances, base rates, fuel surcharge rates, and transit times.

**8. Fuel Purchases:** fuel purchase transactions, gallons purchased, fuel prices, transaction costs, and related vehicle and driver references.

**9. Delivery Events:** pickup and delivery events, scheduled and actual timestamps, detention minutes, and on-time indicators.

**10. Maintenance Records:** maintenance activities, maintenance types, labor and parts costs, total costs, and vehicle downtime.

**11. Safety Incidents:** safety incidents, incident categories, preventability, injuries, vehicle damage, cargo damage, and claims.

**12. Facilities:** facility locations, facility types, dock capacity, coordinates, and operating hours.

**13. Driver Monthly Metrics:** monthly driver metrics, including trips, mileage, revenue, fuel efficiency, fuel consumption, and on-time delivery rate.

**14. Druck Utilization Metrics:** monthly truck metrics, including trips, mileage, revenue, utilization rate, maintenance costs, and downtime.

The source records primarily cover 2022–2024, with a small number of delivery and fuel records extending into January 2025.

## Tools Used
 • Microsoft Excel: Initial data cleaning and preparation.
 
 • Power Query: Data import, transformation, and preparation for analysis.
 
 • Microsoft Power BI: Data modeling, report development, KPI visualization, and interactive dashboard design.
 
 • DAX (Data Analysis Expressions): Development of calculated measures and performance indicators.

## Data Cleaning and Preparation
Data preparation was necessary to organize the source datasets and make them suitable for analysis.
**Microsoft Excel:** Microsoft Excel was used for the initial cleaning and preparation of the data before analysis in Power BI.

**Power Query:** Power Query was used to import and transform the datasets within the Power BI workflow.

 ![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/02fe2ac5d7bc0c028178225353d774c504af3dd0/merged-image%20(2).png)


## Data Modeling
The datasets contain related identifiers, including customer_id, load_id, trip_id, driver_id, and truck_id.
These relationships support the integration of financial and operational data for analysis across customers, loads, trips, drivers, vehicles, maintenance activities, and delivery events.

 ![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/c55968fc04b764b54818eb4d4b6c267b47be3c02/Modelling%20Logistics.PNG)
Modelling

## DAX Measures
DAX was used in the Power BI report to create calculated measures and key performance indicators. The report includes measures for revenue, costs, profit, loads, mileage, delivery performance, driver and fleet performance, and maintenance and safety indicators.

![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/bcbb2095026d47cd3335e40c75beacddf4b3f887/DAX.PNG)
DAX

## Data Analysis
The Power BI report is organized into four dashboard pages.

### 1. Business Overview
The Business Overview dashboard provides a consolidated view of the company’s business performance.
It includes KPIs for revenue, profit, cost, total loads, total miles, and on-time delivery rate.
Additional visuals examine revenue trends, revenue by route, top customers by revenue, and trips by truck make.
This page supports high-level performance monitoring and helps management explore the relationship between financial outcomes and operational activity.

![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/4552c4e03b62ffeb3d7a33069623b39d1f40a187/Business%20Overview.PNG)
Business Overview

### 2. Customers and Revenue
The Customers and Revenue dashboard examines customer contributions and revenue patterns.
Its analytical components include customer-related KPIs, revenue comparisons, revenue by load type, revenue by customer type, and additional charges.
The dashboard supports the evaluation of customer segments and shipment categories to identify important sources of revenue and potential business opportunities.

![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/101f0cbcb069e9d11d3f773adbbb47319daf207e/Customers%20nd%20Revenue.PNG)
Customers and Revenue

### 3. Drivers and Fleet
The Drivers and Fleet dashboard focuses on transportation operations and resource utilization.
Its visuals examine driver performance, trip activity, fuel costs, mileage, fuel efficiency, and fleet utilization.
This page helps management investigate differences in operational performance and identify areas where vehicle and driver resources may be used more effectively.

![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/40e62833199e8202b22e3416ff4b24df32fa5bfa/Drivers%20and%20Fleet.PNG)
Drivers and Fleet

### 4. Maintenance and Safety
The Maintenance and Safety dashboard examines vehicle servicing, maintenance costs, downtime, and safety incidents.
It includes maintenance-related KPIs, maintenance costs by truck make and maintenance type, downtime trends, incident categories, claims, and geographical incident distribution.
The dashboard provides a basis for investigating maintenance requirements, operational risks, and opportunities to improve vehicle reliability and safety.

![image alt](https://github.com/barakatokunlola/Dyrex-Logistics-Analysis/blob/1e1a74b138c222786d0ee9363f795de52a21e00d/Maintenance%20and%20Safety.PNG)
Maintenance and Safety

## Key Insights and Findings
The following findings are based on the financial and operational KPI figures recorded during the project analysis.

**1. Revenue Increased**

The dashboard reported total revenue of 131,967,009.32, compared with 87,732,478.42 in the previous year.
This represents an increase of approximately 50.43%, indicating substantial growth in recorded revenue.

**2. Costs Increased Alongside Revenue**

Total costs increased from 38,314,385.23 in the previous year to 3,926,910.90 in the current period.
This represents an increase of approximately 40.74%.
Although costs increased, their percentage growth was lower than revenue growth over the same comparison.

**3. Profitability Improved**

Total profit increased from 49,418,093.19 to 78,040,098.42, representing growth of approximately 57.93%.
Profit grew faster than both revenue and costs, suggesting an improvement in the reported financial outcome over the comparison period.

**4. Shipment Volume Increased**

The total number of loads increased from 28,546 to 42,946, representing growth of approximately 50.45%.
This indicates a substantial increase in recorded shipment activity.

**5. Total Mileage Increased**

Total miles increased from 40,873,956 to 61,437,750, an increase of approximately 50.31%.
This reflects higher recorded transportation activity and highlights the importance of monitoring fuel efficiency, vehicle utilization, and maintenance costs as mileage increases.

**6. On-Time Delivery Requires Continued Monitoring**

The dashboard reported an on-time delivery rate of approximately 55.20%.
This metric warrants further investigation to understand delivery performance, identify potential causes of delays, and determine where service improvements may be needed.
The interpretation of this percentage should be considered alongside the report’s measure definition and selected filters.

## Summary of Financial and Operational Performance

|KPI    |Previous Year |Current Year   |Approximate Change|
|-------|------------- |-------------- |----------------- |
|Revenue|87,732,478.42 |131,967,009.32 |+50.43%           |
|Cost   |38,314,385.23 |53,926,910.90  |+40.74%           |
|Profit |49,418,093.19 |78,040,098.42  |+57.93%           |
|Loads  |28,546        |42,946         |+50.45%           |
|Miles  |40,873,956    |61,437,750     |+50.31%           |

Note: Percentage changes are calculated from the reported current-year and previous-year figures. Financial and operational values are presented as displayed in the project analysis.

## Recommendations
Based on the findings and the analytical areas covered by the dashboards, the following actions are recommended.

**1. Maintain Focus on Profitable Growth:** Revenue and profit increased during the comparison period. Management should continue monitoring profitability alongside revenue growth to ensure that expansion remains financially sustainable.

**2. Monitor Operating Costs:** As shipment volume and mileage increase, the company should monitor transportation-related expenses, including fuel and maintenance costs. Comparing costs across routes, vehicles, and periods can help identify opportunities for greater efficiency.

**3. Strengthen Customer Performance Monitoring:** Management should review revenue contributions and service performance across customers. This can help identify valuable customer relationships, investigate changes in demand, and support better customer retention strategies.

**4. Improve Fleet Utilization:** Truck utilization, mileage, fuel efficiency, and downtime should be monitored together. Identifying underutilized vehicles or recurring operational inefficiencies can support better fleet allocation and resource planning.

**5. Investigate Delivery Delays:** The reported on-time delivery rate indicates that delivery performance deserves attention. Management should investigate delays by route, driver, facility, and delivery event to identify recurring issues and establish targeted improvements.

**6. Strengthen Preventive Maintenance:** Maintenance records, costs, and downtime should be reviewed to identify recurring repairs and vehicles that require frequent servicing. Preventive maintenance planning may help reduce unexpected downtime and improve fleet availability.

**7. Improve Safety Monitoring:** Safety incidents, preventable accidents, injury indicators, and damage costs should be monitored regularly. Investigating recurring incident patterns can help guide driver training, operational controls, and safety initiatives.

**8. Use the Dashboard for Continuous Monitoring:** The interactive Power BI report can support regular performance reviews by allowing management to examine key indicators and investigate changes across the business.

## Conclusion
The Dyrex Logistics Analysis project demonstrates how multiple logistics datasets can be prepared, connected, and analyzed to create an integrated view of financial and operational performance.

Using Microsoft Excel, Power Query, Power BI, and DAX, the project presents insights into revenue, costs, profitability, shipment volume, mileage, customers, drivers, fleet utilization, maintenance, and safety.The reported results show growth in revenue, profit, load volume, and mileage, while also highlighting the importance of monitoring delivery performance and operating costs.

The four-page dashboard provides a foundation for data-driven decision-making by turning structured logistics data into an interactive reporting solution. This project demonstrates practical skills in data cleaning, data preparation, data modeling, KPI development, DAX calculations, data visualization, and business-focused analysis.


## Skills Demonstrated

 ● Data Cleaning and Preparation
 ● Microsoft Excel
 ● Power Query
 ● Data Modeling
 ● DAX Measures
 ● KPI Development
 ● Year-over-Year Analysis
 ● Data Visualization
 ● Power BI Dashboard Development
 ● Business Intelligence
 ● Data-Driven Decision-Making



