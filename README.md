# cross-department-social-services-analytics
Tableau dashboard analyzing housing, employment, and demographic outcomes using cross-department social services data.

## Overview
This project analyzes client-level data across housing, employment, and demographics to identify patterns that inform public service decision-making.

The dashboard integrates multiple datasets to simulate a cross-department analytics environment.


## Objectives
- Analyze the relationship between housing stability and employment
- Evaluate income patterns across client groups
- Provide demographic context for service populations
- Build a clean, professional Tableau dashboard


## Tools Used
- Tableau (data visualization)
- CSV datasets (data sources)
- Data modeling (relationships between tables)


## Dataset Structure

### Clients
- client_id
- age
- gender
- race
- city

### Employment
- client_id
- employment_status
- income
- job_training

### Housing
- client_id
- housing_status
- rent_amount
- subsidy


## Data Model

The datasets were connected using relationships on a shared key:

A relationship-based model was used instead of joins to preserve data integrity and avoid duplication.


## Dashboard Features

### 1. Employment by Housing Status
- Shows how employment varies across housing conditions

### 2. Average Income (Employed Clients Only)
- Filters out unemployed clients to avoid misleading averages

### 3. Client Demographics by Race
- Provides demographic distribution of clients


## Key Insights

- Stable housing is strongly associated with employment
- All homeless and unstable clients in this dataset are unemployed
- Average income analysis required filtering to employed clients only
- Demographic distribution shows variation across racial groups


## Challenges & Solutions

### Challenge:
Initial dashboard showed missing or misleading data

### Solution:
- Corrected data relationships using `client_id`
- Avoided improper joins
- Applied filters to ensure accurate analysis


## Business Value

- Supports data-driven decision-making across departments
- Highlights risk factors related to housing instability
- Provides insight into client outcomes and service needs
