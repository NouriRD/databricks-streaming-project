# Setup Guide

## Prerequisites

Before running this project, ensure you have:

* A Databricks Free Edition workspace
* Unity Catalog enabled
* A GitHub Personal Access Token (PAT)
* Basic knowledge of Python and SQL

---

## Project Structure

```text
00_config
01_ingestion
02_bronze
03_silver
04_gold
05_dashboard
```

---

## Configuration

Update the following variables inside the configuration notebook:

* Catalog
* Schemas
* Volume path
* GitHub API URL
* GitHub Personal Access Token

---

## Execution Order

Run the notebooks in the following order:

1. project_config
2. github_api_ingestion
3. bronze_streaming
4. silver_transformations
5. gold_kpis

---

## Expected Output

The pipeline creates the following layers:

* Bronze
* Silver
* Gold

Gold tables are ready for analytics and dashboard creation.
