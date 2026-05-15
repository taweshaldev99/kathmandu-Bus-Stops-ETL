# 🚌 Kathmandu Bus Stops ETL Pipeline

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python&logoColor=white)
![Database](https://img.shields.io/badge/Database-SQLite%20%7C%20PostgreSQL-green?logo=postgresql&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-success)

A Python-based **ETL pipeline** project that extracts bus stop data from **OpenStreetMap**, transforms it using **Pandas**, and loads it into an **SQLite database** (extendable to PostgreSQL/MySQL).  
This project was built as part of my application for the ** Training **.

---

## 🚀 Tech Stack

- **Language**: Python (Pandas, Requests, SQLite3, SQLAlchemy)  
- **Data Source**: OpenStreetMap (Overpass API)  
- **Database**: SQLite (transport.db) → extendable to PostgreSQL/MySQL  
- **Libraries**: `pandas`, `requests`

---

## 📂 Project Structure

Dlytica_Project/
│
├── extract_osm_kathmandu.py # Extract data from OpenStreetMap API
├── transform_bus_stops.py # Transform/Clean dataset
├── load_bus_stops.py # Load into SQLite DB
├── query_bus_stops.py # Example queries & analytics
│
├── osm_bus_stops.csv # Raw extracted dataset
├── osm_bus_stops_clean.csv # Cleaned dataset
├── transport.db # SQLite database
│
└── README.md # Documentation

---

## 🗄️ Database Schema

**Table: `bus_stops`**

| Column   | Type    | Description                        |
|----------|---------|------------------------------------|
| id       | INTEGER | Unique bus stop ID (from OSM)      |
| name     | TEXT    | Bus stop name (or "Unknown Stop")  |
| lat      | REAL    | Latitude coordinate                |
| lon      | REAL    | Longitude coordinate               |
| operator | TEXT    | Operating company (if available)   |

---



👨‍💻 Author <br>
Taweshal Dev <br>
📌 GitHub: taweshaldev99 <br>
📧 Email:  thakur2sl.py@gmail.com

