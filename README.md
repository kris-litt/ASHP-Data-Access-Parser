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


## 🚀 Quick Start Instructions

Follow these steps to retrieve the data and convert it for use in Excel:

### 1. Prepare your Environment
* **Navigate to Desktop:** Use the `cd` command to move your terminal pointer to the Desktop.
* **Create a Folder:** Create a NEW FOLDER on the Desktop to hold the 'data' from the API.
* **Rename:** Rename the new folder to something relevant (e.g., `ASHP_Data`).

> *For help with navigation commands, see the [CURL/CD Documentation](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/cd).*

### 2. Fetch the Data
Run the following command in your terminal to save the data directly to a file. 
*Note: Replace `YOUR_API_KEY` with your actual credentials.*

curl "https://ahfs-staging.firebaseio.com/drugShortages.json?auth=YOUR_API_KEY" -o drug_shortages.json


## 3. Convert to Excel
Open the included **HTML** Data Previewer tool.
Upload: Click the selection area (or drag and drop) to select the drug_shortages.json file you just created.
Download: Once the data loads into the viewer, click Download Excel

