# Honda Inventory Scraper

A Flask web app that scrapes used-Honda inventory across multiple Bay Area dealership websites and exports matching listings to CSV.

## What it does

Enter a vehicle model in the web UI, and the app scrapes live inventory from several dealership sites in parallel, pulling title, mileage, price, and listing URL for every matching vehicle. Handles pagination and lazy-loaded content automatically, then bundles results into a downloadable CSV.

## Dealerships covered

- Honda of Stevens Creek (San Jose)
- Honda San Carlos
- Honda of Pasadena
- Additional dealers (Anderson Honda, Capitol Honda, Toyota Palo Alto) wired in but currently disabled

## Stack

- Python, Flask
- Selenium + webdriver-manager (headless Chrome automation)
- CSV export

## Usage

\`\`\`bash
cd Scraper_MAIN
pip install -r requirements.txt
python app.py
\`\`\`

Then open the local web page, pick a model, and download the resulting CSV.

## Status

Functional prototype — built for personal car-shopping comparison across dealers.
