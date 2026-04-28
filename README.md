# NorthStar Databases and Analytics Project

This repository contains the Google Colab notebooks and cleaned datasets for the NorthStar Urban Mobility and Logistics case study.

## Project aim

The aim of this project is to clean, analyse, and prepare the NorthStar dataset for database development and analytics.

## Repository structure

- `notebooks/` contains Google Colab notebooks.
- `data/cleaned_csv/` stores cleaned CSV files.
- `data/json/` stores JSON files prepared for MongoDB.
- `mongodb/` contains MongoDB Atlas and PyMongo notebooks.

## Notebook 01

`01_python_data_cleaning.ipynb` cleans the raw CSV files by:
- checking missing values;
- checking duplicate records;
- standardising inconsistent zone names such as Central, CENTRAL, and Ctr;
- converting date and numeric columns;
- validating values;
- saving cleaned CSV files;
- converting cleaned CSV files to JSON for MongoDB.
