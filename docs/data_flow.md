# Data Flow

This project implements an end-to-end streaming pipeline using the Medallion Architecture.

## Pipeline Flow

```text
GitHub REST API
      │
      ▼
Ingestion Notebook
      │
      ▼
JSON Files
      │
      ▼
Databricks Volume
      │
      ▼
Auto Loader
      │
      ▼
Bronze Layer
      │
      ▼
Silver Layer
      │
      ▼
Gold Layer
      │
      ▼
Dashboard
```

## Layer Description

### Raw Layer

Stores JSON files exactly as received from the GitHub API.

### Bronze Layer

Stores raw streaming data in Delta format.

### Silver Layer

Cleans, transforms and enriches the data.

### Gold Layer

Contains business-ready KPIs used for reporting and dashboards.
