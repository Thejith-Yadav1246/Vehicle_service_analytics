# Vehicle Service Management — Snowflake

## Project Overview

A Snowflake-based Vehicle Service Management and Analytics project that loads vehicle-service data from CSV files stored in Amazon S3, performs data processing and analysis, and demonstrates Snowflake features such as Time Travel and Zero-Copy Cloning.

## Data Sources

The project uses four CSV files:

* `customers.csv` — Customer information
* `vehicles.csv` — Vehicle information
* `service_history.csv` — Vehicle service records
* `parts.csv` — Parts and service-related information

## Technologies Used

* Snowflake
* SQL
* Amazon S3
* GitHub

## Project Workflow

```text
CSV Files
   ↓
Amazon S3
   ↓
Snowflake Stage
   ↓
CSV File Format
   ↓
Snowflake Tables
   ↓
Data Processing & Joins
   ↓
Vehicle Service Analytics
```

## Snowflake Database Structure

**Database:** `VEHICLE_SERVICE_DB`

**Schema:** `SERVICE_ANALYTICS`

The project contains tables for:

* Customers
* Vehicles
* Service History
* Parts

A view is also created for combined service-related analysis.

## Key Operations

The project includes SQL for:

* Creating database objects
* Creating tables
* Creating a CSV file format
* Creating and using stages
* Loading CSV data into Snowflake
* Joining customer, vehicle, service, and parts data
* Calculating service frequency
* Calculating maintenance cost
* Identifying vehicles requiring frequent service
* Creating analytical outputs
* Using Snowflake Time Travel
* Creating a Zero-Copy Clone

## Repository Structure

```text
vehicle-service-management-snowflake/
│
├── CREATIONS.sql
├── OPERATIONS.sql
├── OUTPUT.sql
├── ANALYSIS.sql
└── README.md
```

### SQL Files

**`CREATIONS.sql`**
Contains database, schema, table, and related object creation statements.

**`OPERATIONS.sql`**
Contains file-format, stage, data-loading, and operational SQL commands.

**`OUTPUT.sql`**
Contains project output queries and selected results used for understanding the data.

**`ANALYSIS.sql`**
Contains the final analytical queries used to demonstrate the project requirements.

## Snowflake Features Demonstrated

### Time Travel

Snowflake Time Travel is used to access historical table data and demonstrate recovery/querying of previous data states.

### Zero-Copy Clone

A Zero-Copy Clone is created to demonstrate Snowflake's ability to create a clone of an existing database object without physically copying the underlying data.

## Project Objective

The objective of this project is to demonstrate how Snowflake can be used to ingest, transform, analyze, and manage vehicle service data while applying important Snowflake data-platform features.

## Authors

**B. Thejith**
Government Polytechnic Hyderabad

**T. Mukesh**
Mahaveer Institute of Science and Technology

## Faculty

**Mohammad Jabiulla**
