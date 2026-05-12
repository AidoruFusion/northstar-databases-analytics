# NorthStar Databases and Analytics Project

This repository contains the Google Colab notebooks and datasets for the NorthStar Urban Mobility and Logistics case study.

# Links to Colab
https://drive.google.com/file/d/1OjJlW3RREsP7zkhmLx9tlNWpaZfl12Pm/view?usp=sharing 
https://drive.google.com/file/d/1oPyAqXsMQnPyFTuKhjcx1vC-DO_6XSpz/view?usp=sharing
https://drive.google.com/file/d/1vJUG4LT5KGzmmGEylwpLUcnJA2oWQA8V/view?usp=sharing

## Project aim

The aim of this project is to clean, analyse, and prepare the NorthStar dataset for database development, SQL analysis, MongoDB modelling, and query optimisation.

## Repository structure

- `notebooks/` contains the Google Colab notebooks.
- `data/raw/` contains the original CSV files.
- `data/cleaned/csv/` contains the cleaned CSV files.
- `data/cleaned/json/` contains JSON files prepared for MongoDB.
- `data/analysis/sql_r_outputs/` contains SQL in R output tables, where applicable.

## Workflow

### Notebook 01: Python data cleaning

`Database Assignment.ipynb` cleans the raw CSV files by:

- checking missing values and duplicate records;
- standardising inconsistent zone names such as `Central`, `CENTRAL`, and `Ctr`;
- converting date and numeric columns;
- validating unrealistic or invalid values;
- saving cleaned CSV files;
- converting cleaned CSV files into JSON format for MongoDB.

### Notebook 02: MongoDB Atlas development

`MongoDB_Notebook.ipynb` demonstrates the MongoDB part of the project by:

- connecting Google Colab to MongoDB Atlas using PyMongo;
- uploading cleaned JSON files as collections;
- demonstrating CRUD operations;
- remodelling selected data into an integrated `Operational_Cases` collection;
- creating indexes;
- using `explain()` to review query performance.

### Notebook 03: SQL in R analysis

`R_SQL_Notebook.ipynb` uses R and `sqldf` to query the cleaned datasets by:

- loading cleaned CSV files from the GitHub project folder;
- applying SQL filtering, sorting, grouping, and joins;
- analysing orders, deliveries, complaints, incidents, and driver performance;
- producing outputs that support the final report.

## Summary

The project follows a clear workflow from raw data cleaning to MongoDB database development and SQL-based analysis. The outputs support the NorthStar case study by connecting fragmented operational data and preparing it for evidence-based decision-making.
