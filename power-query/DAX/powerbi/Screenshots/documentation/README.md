#Snow Removal Operations Dashboard

1. Project Objective
   
The objective of this project is to develop a data-driven Power BI dashboard for analyzing snow-removal operations and demonstrating how operational data can be transformed into actionable business insights.

The project focuses on using data analytics to monitor:
•	Snow events and service demand
•	Scheduled versus completed services
•	Crew workload and productivity
•	Service timing and schedule performance
•	Cost per completed service

The project demonstrates an end-to-end analytics workflow from data generation and preparation through data modeling, DAX calculations, visualization, and operational analysis.
________________________________________
2. Business Problem
   
Snow-removal businesses manage multiple crews, properties, equipment, materials, and service schedules during winter operations.
Without a structured data-analysis process, it can be difficult to determine:
•	How much work was completed during each snow event
•	Whether scheduled services were completed on time
•	How workloads were distributed among crews
•	How many crew hours were required
•	What operational costs were associated 
•	Which operational areas may require improvement

The purpose of this project is to demonstrate how a snow-removal company could use operational data to improve visibility into winter-service performance and support better planning and resource management.
________________________________________
3. Data Generation
   
This project uses a synthetically generated dataset created specifically for portfolio and demonstration purposes.

The dataset simulates a realistic winter snow-removal operating environment containing information about snow events, properties, crews, service activities, schedules, and operational costs.

The synthetic data was designed to contain realistic operational variation, including:
•	Multiple snow events
•	Multiple crews
•	Scheduled and actual service times
•	Crew hours
•	Labor costs
•	Service completion status

The dataset does not represent real company, customer, employee, or financial data.

The purpose of generating the data was to create a realistic environment for demonstrating data analytics techniques rather than to report actual business performance.
________________________________________
4. Data Structure
   
The dataset was structured to support analysis of different areas of snow-removal operations.

Key data categories include:
Snow Events Contains information about individual snowfall events.
Examples:
•	Snow Event ID
•	Event Date
•	Snowfall Amount

Crews Contains information about operational crews.
Examples:
•	Crew ID
•	Crew name
•	Crew assignment

Cost Data Operational cost information was used to support analysis of:
•	Labor costs
•	Cost per completed service
________________________________________
5. Data Cleaning and QA/QC
   
The dataset was imported into Power BI using Power Query.

The data-cleaning process included several quality-control checks.
Data Type Validation

Data types were reviewed and standardized.

Examples included:
•	eventDate → EventDate

Duplicate Checks

Records were reviewed for potential duplicate service and event records.

Duplicate records were identified and removed where appropriate.

Missing Value Checks

Important fields were reviewed for missing values, including:
•	Event IDs
•	Crew information
•	Scheduled times
•	Service status
•	Crew hours
•	Cost fields
Standardization

Text fields were standardized to maintain consistency across the dataset.
Examples included:
•	Crew names
•	Service status

Date and Time Validation

Scheduled and actual service times were reviewed to ensure they could be used for schedule-performance analysis.

Operational QA/QC

Additional checks were performed for potentially invalid operational values, including:
•	Negative crew hours
•	Negative equipment hours
•	Negative material quantities
•	Negative costs
•	Invalid service durations
•	Incomplete service records
•	Inconsistent identifiers

Final Validation

After transformation, the cleaned data was reviewed before being loaded into the Power BI data model.

The purpose of the QA/QC process was to improve data consistency and reduce the risk of inaccurate calculations and visualizations.
________________________________________
6. Data Modeling
   
After cleaning the data in Power Query, the tables were loaded into Power BI and organized into a data model.

The data model was designed to allow operational information to be analyzed across multiple dimensions.

The model connects operational service records with information such as:
•	Snow events
•	Crews
•	Dates

Relationships were established using appropriate identifiers such as:
•	Snow Event ID
•	Crew ID
•	Date

A structured data model allows users to filter and analyze operational performance across different dimensions without relying on manually calculated Excel reports.
The model supports analysis such as:
Snow Event → Services → Crew → Costs
This structure provides a foundation for DAX calculations and interactive dashboard analysis.
________________________________________
7. DAX Calculations
   
DAX was used to create measures for operational performance analysis.

The calculations were designed to provide metrics that could be reused across different dashboard pages and filters.
Key analytical measures include:
Total Services

Measures the total number of service records.

Completed Services

Measures the number of services marked as completed.

Completion Rate

Calculates the percentage of services that were completed.

Total Crew Hours

Measures the total amount of crew time used during operations.

Measures crew productivity by comparing completed services with crew hours.

These DAX measures allow the dashboard to respond dynamically to filters such as snow event, crew, service type, and date.
________________________________________
8. Dashboard Design
   
The Power BI dashboard was designed around the operational questions a snow-removal coordinator or manager would need to answer.

Page 1 — Snow Event Overview

Provides a high-level view of winter operations.
Key metrics include:
•	Total snow events
•	Total services
•	Completed services
•	Completion rate
•	Total crew hours

Visualizations can include:
•	KPI cards
•	Snowfall trend
•	Cost by event
•	Service-status breakdown
•	Snowfall
•	Completion
•	Crew hours
•	Costs
•	Crew hours
•	Completion rate
•	Completion performance

Interactive slicers allow users to filter the dashboard by relevant dimensions such as date, snow event, crew, property, and service type.

10. Key Findings
    
The Power BI dashboard provides several operational insights from the simulated snow-removal dataset.

9.1 Snowfall and Event Activity

The dataset contains 45 snow events with a combined snowfall total of 564.50 cm.

The heaviest recorded snowfall event was 22.00 cm.

This indicates substantial variation in snowfall intensity across events, creating different levels of operational demand.

9.2 Service Completion

The dashboard reports a 77.78% completion rate.

The service-status distribution shows approximately:
•	35 completed events
•	8 scheduled events
•	2 standby events

The difference between completed and non-completed events provides an opportunity to examine workload, scheduling, crew availability, and operational capacity.

9.3 Labor Utilization

A total of 148 labor hours were recorded across the snow events.

Labor utilization was distributed between the two crews:
•	Crew A: 66 hours
•	Crew B: 82 hours

Crew B accounted for approximately 55.4% of recorded labor hours, while Crew A accounted for approximately 44.6%.

This provides an initial indication that Crew B carried a larger share of the simulated workload.

The event-cost visualization also shows substantial variation in cost between snow events, indicating that individual events can require significantly different levels of operational resources.

9.4 Crew Workload

The difference between Crew A's 66 labor hours and Crew B's 82 labor hours demonstrates that labor was not distributed equally between the two crews.

This provides an opportunity for further analysis of:
•	Number of services completed by each crew
•	Crew productivity
•	Cost per crew
•	Workload by snow event

9.5 Overall Operational Performance

The dashboard demonstrates that the simulated operation experienced a mixture of completed, scheduled, and standby work.

The 77.78% completion rate, 148 labor hours, and approximately $47,702 in event costs provide a useful baseline for evaluating operational performance.

The dashboard can therefore be used as a management tool to investigate where additional resources, scheduling adjustments, or workload balancing may be required.


