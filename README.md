# Production-Line-Data-Analysis

This repository contains code for analyzing production line data using Python and SQLite. It includes scripts to upload and process CSV files, execute SQL queries to count entries, and calculate NiO, iO, and warning counts per station. Additionally, it provides visualizations of var2 values over time with daily average calculations and interpolations for missing data points.

## Google Colab
- Upload your CSV-file possible with Google Colab

## Features
- Upload and process CSV files
- Store data in SQLite database
- Execute SQL queries to count total entries, NiOs, iOs, and warnings per station
- Calculate NiO rates per station
- Calculate and plot daily average of var2 values with interpolated missing data points

## Issues and Resolutions
### Problem 1: Incorrect Data Types for result
Issue: The result column in the CSV file was read as strings, including 'warning', instead of integers. => Resolution: Convert 'warning' to a numeric value and ensure the result column is numeric.
### Problem 2: Displaying Only NiOs and iOs
Issue: The initial queries only counted NiOs (result=1) and iOs (result=0), missing warnings. => Resolution: Added a query to count warnings (result='warning') and included it in the final output.
### Problem 3: Time Series Plotting with Missing Dates
Issue: The time series plot had gaps for dates without entries. => Resolution: Created a complete date range and interpolated missing var2 values.

## Requirements
- Python 3.x
- pandas
- sqlite3
- matplotlib

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/production-line-data-analysis.git
   cd production-line-data-analysis
