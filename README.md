# SQL_Investigative-_Analysis
## Project Overview
This project is a data-driven investigative analysis of a documented case involving the murder of Roland Greene, a well-known art collector, who was found dead in his private estate. Using SQL, timelines, and structured reports, the goal is to identify inconsistencies, verify statements, and highlight key findings from the available data.
The dataset includes timelines of events, guest statements, and related documentation. Analytical queries were written to examine relationships, detect discrepancies, and uncover insights from the structured information.

## Case Summary
- Victim: Roland Greene (Art Collector)
- Location: Vault Room, Private Estate
- Time of Death: 8:00 PM
- Last Contact: Phone call received at 7:55 PM
- Suspects: 30 guests, all claiming alibis
- Analytical Challenge: Only one suspect’s statement is inconsistent.

## Data Overview
The dataset contains investigative information, including false alibis reported by guests, inconsistencies across statements and timelines, and overlapping events, to support analysis and uncover key insights from the case.
|Datasets|Description|
|---------|-----------|
|Suspects_large.csv (30 records)|Suspect profiles with roles, relationships, and alibis|
|Call_records_large.csv (90 records)|Phone call history including calls to the victim|
|Access_logs_large.csv (100 records)|Door access records from the estate security system|
|Forensic_events_large.csv (5 records)|Timeline of critical forensic events|

## Analytical Approach
### 1. Data Preparation and Cleaning
The raw CSV file was imported into Microsoft SQL Server, and the dataset was prepared for analysis by:
- Validating the database schema, timestamps, and constraints.
- Standardizing inconsistent formats across tables.
- Ensuring data integrity for subsequent SQL queries and analysis.

  ### 2. Exploratory Analysis
   During EDA, the dataset was examined to uncover patterns, inconsistencies, and potential leads:
- Reviewed suspect alibis for logical inconsistencies.
- Analyzed door access patterns and movement behavior throughout the course of event.
- Cross-referenced phone call logs with the forensic timeline to verify reported activities.
This step helped identify anomalies and provided insights to guide further investigation and scoring.

### 3. 



