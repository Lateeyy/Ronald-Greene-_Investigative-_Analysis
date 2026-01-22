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

### 3. Suspicious Scoring System
A multi-factor scoring framework was developed to rank suspects based on potential inconsistencies and risk indicators:
- Vault access during critical time windows.
- Communication with the victim shortly before the incident.
- Contradictions between stated alibis and actual activity.
- Relationship-based motive indicators.
- Abnormal movement frequency within the estate.
This framework allowed the team to quantitatively evaluate suspect statements and behavior, highlighting individuals with higher likelihoods of providing false information.

### 4. Timeline Reconstruction
The timeline of events was reconstructed to validate suspect statements and identify discrepancies:
- Reviewed and mapped each suspect’s location minute by minute.
- Identified contradictions between alibis and actual locations.
- Detected overlapping events and impossible alibis.
- Narrowed the suspect pool by focusing on critical time windows.

## Key Findings  
- Timeline reconstruction identified a critical window around 20:00, during which the incident occurred.
- Access log analysis revealed that only a small subset of suspects entered the Vault Room shortly before or after the critical time window.
- Cross-referencing alibi statements with access and movement logs showed that multiple suspects provided false or contradictory alibis.
- One suspect was identified as the only individual to meet all high-risk criteria, including vault access proximity, false alibi, and abnormal movement patterns.
- Door access records showed failed entry attempts followed by successful access, suggesting deliberate effort to gain entry to restricted areas.
- Phone call records and forensic timelines revealed inconsistencies and overlapping events, indicating possible data manipulation or post-incident activity.
- Combined analysis significantly narrowed the suspect pool, highlighting a primary subject for further investigation.

## SQL Skills Demonstrated
- Advanced JOIN Operations: Combined multiple tables (access logs, alibis, timelines) to accurately reconstruct suspect movements and interactions.
- Logical Operations: Used conditional logic (CASE, boolean operators) to detect false alibis and eliminate impossible timelines.
- Common Table Expressions (CTEs): Structured complex forensic queries into readable, step-by-step analytical layers.
- Window Functions: Applied ranking and sequencing functions to analyze suspect activities within critical time windows.
- Date & Time Analysis: Performed precise timestamp comparisons to identify actions occurring around the time of death.
- Subqueries, Aggregation & Scoring: Built a multi-factor scoring and ranking model to prioritize suspects based on behavioral risk indicators.




