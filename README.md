# ⚡ Power Grid Data Scraper

This Python script scrapes **power generation data** from the [Bangladesh Power Grid Company ERP portal](https://erp.powergrid.gov.bd/web/generations/view_generations) and saves the extracted information from all pages into a CSV file.

---

## 🧩 Overview

The script automatically:
- Iterates through **1776 pages** of data from the ERP portal.  
- Extracts table rows and columns (first 4 columns per row).  
- Writes all data into a single CSV file (`all_pages_data.csv`).  
- Uses connection pooling for efficiency and adds delay between requests to avoid overwhelming the server.

---

## ⚙️ Features

✅ Handles pagination automatically  
✅ Gracefully skips missing or invalid pages  
✅ Saves data incrementally to prevent data loss  
✅ Uses `BeautifulSoup` for HTML parsing  
✅ Adds polite delay between requests  
✅ Disables SSL verification warnings safely  

---

## 🧠 Requirements

You’ll need the following Python packages:

```bash
pip install requests beautifulsoup4 urllib3
