# System Logs Analytics Pipeline - Eventify
![screenshot of app](2tierDeployment.png)

Eventify’s platform generates application log files capturing user actions such as logins,
event creation,location, user device and errors. These logs are currently generated from
servers, stored as csv files locally and are primarily used by engineers for system
understanding.


## Problem Statement

- Application logs are:
  Stored as raw, csv files
  Difficult to query or analyze
  Not centrally available for analytics teams
  Inconsistent in formatting and occasionally malformed

## Challenges 
 -Analysts cannot answer basic questions (e.g., daily logins, error rates)
Product teams lack visibility into user behavior
Operations teams manually inspect logs during incidents
The company needs a reliable ETL pipeline to convert raw log files into a structured event
table stored in a database.

##  Project Objectives
 - Extracts raw application log files
 - Parses and cleans log data
 -  Handles invalid or corrupt log entries gracefully
 -  Loads clean, structured events into a relational database
 - Produces an analytics-ready event table
 

##  Rationale for the Project

 - This project mirrors a data engineering problem where:
 - Data is not clean and analytically acceptable
 - Input files may contain errors
 - Data must be made usable for downstream teams