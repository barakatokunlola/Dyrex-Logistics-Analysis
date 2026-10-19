# Dyrex Logistics Analysis 

## Introduction
The Dyrex Logistics Analysis project explores the financial and operational performance of a logistics company using Microsoft Power BI. The project combines multiple datasets covering loads, customers, routes, trips, drivers, trucks, fuel purchases, delivery events, maintenance records, and safety incidents.
The objective is to transform raw operational data into meaningful insights that support business performance monitoring, revenue analysis, fleet management, delivery performance evaluation, maintenance planning, and safety monitoring.
The analysis was developed using Microsoft Excel, Power Query, Power BI, and DAX and presented through a four-page interactive dashboard.
Problem Statement
Logistics operations involve several interconnected activities, including customer management, shipment processing, revenue generation, transportation, fuel consumption, fleet utilization, vehicle maintenance, and delivery scheduling.
Without a consolidated reporting solution, it can be difficult for management to monitor these activities, understand performance trends, identify operational risks, and make informed decisions.
Dyrex Logistics requires an integrated view of its financial and operational performance to understand revenue generation, evaluate fleet and driver activities, monitor delivery reliability, and assess maintenance and safety performance.
This project addresses these needs by preparing and analyzing multiple logistics datasets and presenting the results through an interactive Power BI dashboard.
Business Questions
1. Business Overview
 • What are the company’s overall revenue and operational activity levels?
 • How does revenue vary over time?
 • Which customers, routes, and truck makes contribute to business activity?
 • How many loads and trips are recorded?
 • What proportion of delivery events are completed on time?
 • How can financial and operational KPIs support management decisions?
2. Customers and Revenue
 • Which customers generate the highest revenue?
 • How is revenue distributed across customer types?
 • How do Dry Van and Refrigerated loads compare in volume and revenue?
 • How do booking arrangements contribute to revenue?
 • What additional charges and fuel surcharges are associated with loads?
 • Which customer segments may offer opportunities for improved revenue generation?
3. Drivers and Fleet
 • How many trips are recorded across the fleet?
 • How do driver revenue and operational performance vary?
 • How effectively are trucks being utilized?
 • What patterns exist in mileage and fuel efficiency?
 • How do fuel costs vary across drivers and fleet operations?
 • Which areas may require further investigation to improve fleet efficiency?
4. Maintenance and Safety
 • What are the total recorded maintenance costs and downtime?
 • Which maintenance categories account for the highest costs?
 • How does maintenance downtime change over time?
 • How many safety incidents have been recorded?
 • Which incident categories account for the most incidents and claims?
 • How can maintenance and safety data support better operational risk management?
Data Source
The project uses a ZIP archive containing 14 CSV datasets and a Key Guide.docx document.
The datasets cover the following areas:
Dataset
Purpose
loads.csv
Contains shipment records, load dates, load types, customers, routes, revenue, fuel surcharges, additional charges, and load status.
customers.csv
Contains customer information, customer types, account status, freight preferences, credit terms, and annual revenue potential.
trips.csv
Contains trip records, assigned drivers and vehicles, dispatch dates, distance, duration, fuel consumption, and trip status.
drivers.csv
Contains driver information, employment status, experience, license details, and home terminals.
trucks.csv
Contains truck information, makes, model years, fuel types, acquisition details, and vehicle status.
trailers.csv
Contains trailer inventory, trailer types, specifications, acquisition details, and status.
routes.csv
[10/19/2026 10:09 AM] Dyra: Contains route origins and destinations, typical distances, base rates, fuel surcharge rates, and transit times.
fuel_purchases.csv
Contains fuel purchase transactions, gallons purchased, fuel prices, transaction costs, and related vehicle and driver references.
delivery_events.csv
Contains pickup and delivery events, scheduled and actual timestamps, detention minutes, and on-time indicators.
maintenance_records.csv
Contains maintenance activities, maintenance types, labor and parts costs, total costs, and vehicle downtime.
safety_incidents.csv
Contains safety incidents, incident categories, preventability, injuries, vehicle damage, cargo damage, and claims.
facilities.csv
Contains facility locations, facility types, dock capacity, coordinates, and operating hours.
driver_monthly_metrics.csv
Contains monthly driver metrics, including trips, mileage, revenue, fuel efficiency, fuel consumption, and on-time delivery rate.
truck_utilization_metrics.csv
Contains monthly truck metrics, including trips, mileage, revenue, utilization rate, maintenance costs, and downtime.
The accompanying Key Guide.docx documents the database structure, primary keys, foreign keys, table relationships, and suggested analytical use cases.
The source records primarily cover 2022–2024, with a small number of delivery and fuel records extending into January 2025.
Tools Used
 • Microsoft Excel: Initial data cleaning and preparation.
 • Power Query: Data import, transformation, and preparation for analysis.
 • Microsoft Power BI: Data modeling, report development, KPI visualization, and interactive dashboard design.
 • DAX (Data Analysis Expressions): Development of calculated measures and performance indicators.
 • GitHub: Project documentation and portfolio presentation.
Data Cleaning and Preparation
Data preparation was necessary to organize the source datasets and make them suitable for analysis.
Microsoft Excel
Microsoft Excel was used for the initial cleaning and preparation of the data before analysis in Power BI.
Power Query
Power Query was used to import and transform the datasets within the Power BI workflow.
Data Modeling
The datasets contain related identifiers, including customer_id, load_id, trip_id, driver_id, and truck_id.
The Key Guide.docx was used to understand the database schema and the intended relationships between tables.
These relationships support the integration of financial and operational data for analysis across customers, loads, trips, drivers, vehicles, maintenance activities, and delivery events.
DAX Measures
DAX was used in the Power BI report to create calculated measures and key performance indicators.
The report includes measures for revenue, costs, profit, loads, mileage, delivery performance, driver and fleet performance, and maintenance and safety indicators.
Data Analysis
The Power BI report is organized into four dashboard pages.
1. Business Overview
The Business Overview dashboard provides a consolidated view of the company’s business performance.
It includes KPIs for revenue, profit, cost, total loads, total miles, and on-time delivery rate.
Additional visuals examine revenue trends, revenue by route, top customers by revenue, and trips by truck make.
This page supports high-level performance monitoring and helps management explore the relationship between financial outcomes and operational activity.
2. Customers and Revenue
The Customers and Revenue dashboard examines customer contributions and revenue patterns.
Its analytical components include customer-related KPIs, revenue comparisons, revenue by load type, revenue by customer type, and additional charges.
The dashboard supports the evaluation of customer segments and shipment categories to identify important sources of revenue and potential business opportunities.
3. Drivers and Fleet
The Drivers and Fleet dashboard focuses on transportation operations and resource utilization.
Its visuals examine driver performance, trip activity, fuel costs, mileage, fuel efficiency, and fleet utilization.
[10/19/2026 10:09 AM] Dyra: This page helps management investigate differences in operational performance and identify areas where vehicle and driver resources may be used more effectively.
4. Maintenance and Safety
The Maintenance and Safety dashboard examines vehicle servicing, maintenance costs, downtime, and safety incidents.
It includes maintenance-related KPIs, maintenance costs by truck make and maintenance type, downtime trends, incident categories, claims, and geographical incident distribution.
The dashboard provides a basis for investigating maintenance requirements, operational risks, and opportunities to improve vehicle reliability and safety.
Key Insights and Findings
The following findings were calculated from the supplied CSV datasets. They describe the source data and are not presented as independent reproductions of every filtered Power BI measure.
1. The Dataset Contains 85,410 Loads
The loads.csv dataset contains 85,410 load records.
The records are distributed across two load types:
Load Type
Number of Loads
Recorded Revenue
Refrigerated
42,946
131,967,009.32
Dry Van
42,464
130,558,790.97
Total
85,410
262,525,800.29
Refrigerated loads account for approximately 50.28% of all recorded loads and generate slightly more revenue than Dry Van loads.
The revenue values are presented as recorded in the source dataset; the CSV schema does not explicitly specify the currency.
2. First Group Is the Highest-Revenue Customer in the Source Data
Aggregating the revenue field in loads.csv by customer identifies First Group as the highest-revenue customer.
Its recorded revenue is approximately 9,136,680.18.
The next four highest-revenue customers are:
Customer
Recorded Revenue
First Group
9,136,680.18
First Logistics
6,384,063.99
Metro Wholesale
5,408,237.57
XYZ Wholesale
5,282,241.66
Continental Supply Chain
5,227,446.48
These figures are based on the raw load revenue field and may differ from dashboard results if report filters or additional revenue components are applied.
3. Dedicated Bookings Account for the Largest Revenue Total by Booking Type
Aggregating recorded revenue by booking_type produces the following results:
Booking Type
Number of Loads
Recorded Revenue
Dedicated
42,337
130,236,635.41
Spot
21,528
66,321,705.72
Contract
21,545
65,967,459.16
Dedicated bookings account for approximately 49.61% of total recorded load revenue.
This indicates that dedicated bookings are a major contributor to revenue in the supplied data.
4. Delivery Events Show a Clear Difference Between Pickup and Delivery Timeliness
The delivery_events.csv dataset contains 170,820 event records.
Calculating the proportion of events marked on time gives:
Event Type
Number of Events
On-Time Rate
Pickup
85,410
66.73%
Delivery
85,410
44.61%
All Events Combined
170,820
55.67%
The delivery on-time rate is approximately 22.12 percentage points lower than the pickup on-time rate.
This is an important operational finding. It suggests that delivery performance deserves closer investigation.
It also demonstrates why the definition of an on-time KPI matters: combining pickup and delivery events produces a different result from calculating the rate using delivery events alone.
5. The Maintenance Dataset Contains 2,920 Records
The maintenance_records.csv dataset contains 2,920 maintenance records.
Aggregating the total_cost and downtime_hours fields gives:
 • Total recorded maintenance cost: 5,730,573.28
 • Total recorded maintenance downtime: 72,230.5 hours
Preventive maintenance accounts for the highest total cost among the maintenance categories in this dataset.
Maintenance Type
Number of Records
Total Cost
Preventive
422
963,576.34
Repair
424
945,375.44
Tire
414
919,413.24
Brake
402
911,667.23
Engine
415
890,537.88
Transmission
411
879,620.87
Inspection
432
220,382.28
Inspection has the lowest recorded total maintenance cost, while preventive maintenance has the highest.
These totals come from the maintenance records themselves. They should not be added to the monthly fleet utilization maintenance totals because the two datasets represent related measures and may overlap.
6.
[10/19/2026 10:09 AM] Dyra: The Safety Dataset Contains 170 Incidents
The safety_incidents.csv dataset contains 170 recorded safety incidents.
The data includes:
 • 64 preventable incidents, representing approximately 37.65% of recorded incidents.
 • 33 incidents with an injury indicator.
 • 2,653,171.82 in total recorded claims.
The incident categories also show different cost patterns.
DOT Violations account for the largest number of incidents, with 39 records. Equipment Damage has the highest aggregate claim amount, at approximately 740,970.73.
These results suggest that management should consider both incident frequency and financial impact when evaluating safety risks.
7. The Project Covers Multiple Connected Operational Resources
The source files contain:
Resource
Number of Records
Customers
200
Drivers
150
Trucks
120
Trailers
180
Routes
58
Facilities
50
Loads
85,410
Trips
85,410
Delivery Events
170,820
Fuel Purchases
196,442
The breadth of these datasets makes it possible to examine logistics operations from multiple perspectives rather than relying on a single table.
The data also highlights the importance of understanding table relationships and avoiding double counting when combining transaction-level records with monthly summary metrics.
Recommendations
Based on the verified source-data findings and the analytical scope of the dashboards, the following actions are recommended.
1. Investigate Delivery Delays
The delivery event data shows a lower on-time rate for deliveries than for pickups.
Management should investigate delays by route, facility, driver, and delivery event to identify recurring issues and prioritize improvements.
2. Monitor Revenue by Customer and Booking Type
First Group is the highest-revenue customer in the source data, while dedicated bookings contribute the largest revenue total by booking type.
Management should monitor revenue concentration, customer retention, and service performance to maintain valuable relationships and reduce overdependence on a small number of customers.
3. Evaluate Load-Type Performance
Refrigerated and Dry Van loads generate broadly similar total revenue in the source data.
Management should compare their operating costs, service requirements, and profitability before deciding where to allocate additional resources.
4. Review Maintenance Costs and Downtime
Preventive maintenance accounts for the highest recorded maintenance cost by category.
Management should evaluate whether this spending is associated with reduced breakdowns and downtime. Maintenance costs should be considered alongside vehicle availability and operational reliability rather than assessed in isolation.
5. Strengthen Safety Management
With 170 recorded incidents and 64 marked as preventable, safety performance warrants continued attention.
Management should review preventable incidents, investigate recurring incident categories, and use claims and damage costs to guide targeted safety interventions.
6. Monitor Fuel Efficiency and Fleet Utilization
Fuel consumption, mileage, and utilization should be reviewed together to identify opportunities to improve vehicle efficiency.
Comparisons across trucks and drivers may help identify operational patterns that require further investigation.
7. Standardize KPI Definitions
Management should establish consistent definitions for revenue, total cost, profit, load volume, mileage, and on-time delivery rate.
For example, delivery punctuality should be measured using delivery events when the intended KPI is specifically about on-time deliveries. This helps prevent misleading comparisons and improves confidence in management reporting.
Conclusion
The Dyrex Logistics Analysis project demonstrates how multiple datasets can be prepared, connected, and analyzed to provide a broader understanding of logistics performance.
Using Microsoft Excel, Power Query, Power BI, and DAX, the project explores customer revenue, booking types, shipment activity, driver and fleet performance, fuel consumption, maintenance costs, delivery timeliness, and safety incidents.
[10/19/2026 10:09 AM] Dyra: The source-data analysis identifies First Group as the highest-revenue customer, dedicated bookings as the largest contributor to recorded revenue by booking type, a lower on-time rate for deliveries than pickups, and meaningful maintenance and safety costs.
The four-page Power BI dashboard organizes these analytical areas into an interactive reporting solution that supports business performance monitoring and further investigation.
This project demonstrates practical skills in data cleaning, data transformation, data modeling, KPI development, DAX, data visualization, and business-focused analysis.
Project Files
 • Source Data: ZIP archive containing 14 CSV datasets and the database Key Guide.
 • Power BI Report: Dyrex Logistics Analysis.pbix
 • Project Documentation: README.md
Skills Demonstrated
 • Microsoft Excel
 • Power Query
 • Data Cleaning and Preparation
 • Data Modeling
 • DAX Measures
 • KPI Development
 • Customer and Revenue Analysis
 • Fleet and Driver Analysis
 • Maintenance and Safety Analysis
 • Data Visualization
 • Power BI Dashboard Development
 • Business Intelligence
 • Data-Driven Decision-Making
