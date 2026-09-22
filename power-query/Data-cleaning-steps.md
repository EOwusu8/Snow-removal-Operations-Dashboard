#Power Query — Data Cleaning Steps

#Data Import

The synthetic snow-removal operations dataset was imported into Microsoft Excel using Power Query.

#Data Type Validation

Column data types were reviewed and corrected where necessary.

Example include:
•	eventDate → EventDate

#Duplicate Check

Records were reviewed for duplicate snow-event and service records.

#Missing Value Check

Columns were reviewed for missing values, including:
•	Snow event ID
•	Crew
•	Actual time
•	Service status
•	Crew hours
•	Event date
5. Standardization

Text fields were standardized to ensure consistent grouping and reporting.

Examples include:
•	Crew names
•	Service status
•	Snow Event ID

#Date and Time Validation

Event dates and times were reviewed to identify invalid or inconsistent records.

#Operational Validation

Operational values were reviewed for unrealistic or invalid values.

Examples include:
•	Negative crew hours
•	Negative costs
•	Invalid service times

#QA/QC

The transformed tables were reviewed before being loaded into the Power BI data model.

The objective was to ensure that the dataset was consistent, appropriately typed, and suitable for analysis.

#Output

The cleaned tables were loaded into Power BI for:
•	Data modeling
•	Relationship creation
•	DAX calculations
•	Dashboard development
•	Operational analysis

