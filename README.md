# ASHP Data Access & Parser

This repository contains scripts and documentation for accessing and formatting drug shortage data from the American Society of Health-System Pharmacists (ASHP). This project was developed to bridge the gap between raw API/Terminal data retrieval and academic data analysis.

## Overview
The project focuses on:
* **Data Retrieval:** Using `curl` commands to bypass browser-based access issues and interface directly with the ASHP data source.
* **Troubleshooting:** Documenting solutions for "Permission Denied" errors and API key authentication hurdles.
* **Data Transformation:** Converting complex JSON payloads into structured CSV/Excel files for use in pharmaceutical research.

## Project Structure
* `/data`: (Optional) Sample data or templates.
* `/scripts`: Python or Shell scripts used to fetch and parse the data.
* `/docs`: Technical troubleshooting logs regarding API connectivity.

## Getting Started
### Prerequisites
* Terminal/CLI access
* (Optional) Python 3.x for parsing scripts

### Usage
To fetch the raw JSON data, use the following terminal command format:
```bash
curl -H "Authorization: Your_API_Key" [ASHP_Endpoint_URL] -o raw_data.json
