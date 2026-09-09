# hemodynamics-inventory-automation
Python-based ETL tool for medical device cross-referencing and automated inventory logging in Cath Labs.

A specialized Python automation tool developed for **Cath Lab (Hemodynamics)** environments to optimize the management of medical device catalogs and inventory logging.

## The Problem
Medical staff often struggle with manual, time-consuming lookups in fragmented PDF catalogs to find specific billing codes and device specifications. This tool solves that by automating the search and registration process for high-value assets like Stents and Balloons.

## Key Technical Features
- **Intelligent Filtering:** Uses Regular Expressions (RegEx) to distinguish between precise medical sizes (e.g., matching '4Fr' while ignoring '4.5' or ranges).
- **Data Normalization:** Processes Spanish medical terminology and accents for a resilient search engine.
- **Automated Excel Integration:** Dynamically logs usage data into vendor tracking spreadsheets using `OpenPyXL`.
- **Session Intelligence:** Tracks session statistics for shift-end reporting without manual counting.

## Impact
Reduces administrative lookup and logging time by approximately **70%**, minimizing human error in billing and high-cost material tracking.

## Tech Stack
- **Python 3.10+**
- **Libraries:** `pdfplumber` (PDF parsing), `openpyxl` (Excel automation), `re` (Pattern matching).

## Installation
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run: `python inventory_manager.py`

---
*Developed as part of a real-world solution for clinical workflow optimization.*
