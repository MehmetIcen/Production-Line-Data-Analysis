# Production-Line-Data-Analysis

This repository contains code for analyzing production line data using Python and SQLite. It includes scripts to upload and process CSV files, execute SQL queries to count entries, and calculate NiO, iO, and warning counts per station. Additionally, it provides visualizations of var2 values over time with daily average calculations and interpolations for missing data points.

## Features
- Upload and process CSV files
- Store data in SQLite database
- Execute SQL queries to count total entries, NiOs, iOs, and warnings per station
- Calculate NiO rates per station
- Calculate and plot daily average of var2 values with interpolated missing data points

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
