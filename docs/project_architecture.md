# Project Architecture

## Overview

This project demonstrates a modern streaming data pipeline built with Databricks and Delta Lake.

The architecture follows the Medallion Architecture pattern.

## Components

### GitHub REST API

Provides real-time public GitHub events.

### Databricks Volume

Stores raw JSON files collected from the API.

### Auto Loader

Automatically detects and ingests new files.

### Bronze Layer

Stores raw Delta tables.

### Silver Layer

Applies data cleaning and transformations.

### Gold Layer

Creates aggregated KPI tables for analytics.

### Dashboard

Visualizes business metrics using Databricks SQL.
