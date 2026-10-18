# divvy-bike-sharing-analysis
End-to-end analysis of 3.3M+ Divvy bike-sharing trips using Python, SQL and Power BI, with a focus on data quality, rider behaviour and operational insights.

# Divvy Bike Sharing Analysis

## Overview

This project analyzes more than 3.3 million Divvy bike-sharing trips from January to July 2026.
The goal of the project is to explore rider behaviour, identify usage patterns, perform data quality checks, and prepare the data for business-oriented reporting.
The analysis covers the full data workflow: data exploration, cleaning and validation in Python, SQL analysis using DuckDB, and Power BI reporting.
**Status:** In Progress — Python data preparation and SQL analysis are completed. The Power BI dashboard is currently under development.

---

## Tools

- Python
- Pandas
- SQL
- DuckDB
- Power BI
- Power Query
- Jupyter Notebook

---

## Dataset

The project is based on Divvy bike-sharing trip data for the period:
**January 2026 – July 2026**

Initial dataset:
- 3,389,831 records
- 13 original columns

Final cleaned dataset:
- 3,297,649 records
- 21 columns

---

## Data Cleaning & Quality Checks

The dataset was explored, cleaned and validated using Python and Pandas.

The main data quality checks included:
- checking duplicate ride IDs
- removing duplicate records
- validating trip dates
- checking missing values
- identifying incomplete station information
- validating ride duration
- removing trips shorter than 1 minute
- removing trips longer than 24 hours
- preparing additional variables for analysis

After cleaning, 3,297,649 trips remained in the final dataset.
Additional variables were created, including:

- start date
- month
- month name
- day of week
- hour of day
- weekend indicator
- ride duration

---

## SQL Analysis

SQL analysis was performed using DuckDB.
The analysis focused on:
- overall trip volume
- member vs casual rider behaviour
- monthly ridership trends
- weekday vs weekend usage
- hourly usage patterns
- bike type preferences
- most popular start stations
- most popular routes
- round-trip behaviour
- ride duration differences

---

## Key Findings

- Members account for approximately 65% of all trips.
- Casual riders have longer average ride durations than members.
- Member usage shows strong morning and evening peaks, consistent with commuting-related behaviour.
- Casual riders are more active during weekends.
- Casual riders use electric bikes more frequently than members.
- Round trips are significantly more common among casual riders.
- Ridership increased substantially between January and July 2026.
- Navy Pier was the most popular starting station during the analyzed period.

---

## Power BI Dashboard

The Power BI dashboard is currently under development.
The dashboard will include:

- total rides and key KPIs
- monthly ridership trends
- rider type distribution
- hourly usage patterns
- weekday and weekend analysis
- top stations
- bike type preferences
- round-trip behaviour

---

## Project Structure

```text
divvy-bike-sharing-analysis/
│
├── 01_data_exploration.ipynb
├── 02_data_cleaning.ipynb
├── 03_sql_analysis.ipynb
├── README.md
└── .gitignore
