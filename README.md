# Marketing Leads Dashboard — Santiago RD

A Streamlit dashboard that scans multiple data sources (Google Search, Booking, Airbnb, Visit Santiago, Instagram) to estimate search volume, clicks, and generated leads for the tourism/hospitality market in Santiago de los Caballeros, Dominican Republic.

## Features

- Multi-source data scanning configuration
- Automatic lead scoring and categorization (High/Medium/Low)
- Results stored in Google Sheets via the Sheets API
- Historical segment analysis using K-Means clustering
- Interactive visualizations with Plotly

## Tech Stack

Python, Streamlit, Pandas, Scikit-learn (K-Means), Plotly, BeautifulSoup, Google Sheets API (gspread), Docker

## Setup

Requires a Google Service Account JSON key (not included in this repo for security) mounted at `/app/credenciales_google.json`, with access to a Google Sheet named `Reporte_IA_Santiago`.

```bash
docker build -t marketing-dashboard .
docker run -p 8000:8000 marketing-dashboard
```
