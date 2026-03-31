# COMP 3610 Assignment 3

## Overview
An intelligent data analytics system combining Apache Spark for distributed 
data processing and a RAG pipeline for natural language querying over NYC 
transportation policy documents.

## Preface 
Spark was not running locally so Part 1 was done in Collab, then the rest of the Parts locally 

## Project Structure
- `assignment3.ipynb` — Main Jupyter notebook with all code and outputs
- `docs/` — Curated PDF document corpus
- `requirements.txt` — Python dependencies
- `.gitignore` — Excludes data files and generated artifacts

## Dataset
NYC Yellow Taxi Trip Records (January 2024) — downloaded programmatically:
```python
import urllib.request
url = "https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2024-01.parquet"
urllib.request.urlretrieve(url, "yellow_tripdata_2024-01.parquet")
```

## Document Corpus (docs/)
- `annual_report_2023.pdf` — NYC TLC Annual Report 2023
- `NYC-Vision-Zero-Investment.pdf` — Vision Zero Investment Report
- `stratplan_compplan.pdf` — NYC DOT Sustainable Streets Strategic Plan
- `25-38 NYC Delivery Worker Data Collection and Research Report.pdf` — NYC Delivery Worker Research
- `mta-annual-report-2023.3.pdf` — Motor Trade Association Annual Report 2023

## Setup Instructions
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Download the taxi data using the code above
4. Open `assignment3.ipynb` in Jupyter or Google Colab
5. Run all cells top to bottom

## LLM Server
This project uses the COMP 3610 course LLM server with model 
`llama3-8b-instruct`
