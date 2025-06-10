# Public Transport Reliability-analysis
This project analyzes the reliability of public bus transportation using PostgreSQL. It focuses on on-time performance, delay causes (like weather), and feedback ratings. The goal is to provide meaningful insights for improving public transport systems using SQL only.

🧰 Tech Stack
PostgreSQL (v14 or higher recommended)
pgAdmin (or any SQL GUI)
CSV files for data import
🧱 Database Schema

1. routes
route_id (PK)
origin
destination
distance_km

2. buses
bus_id (PK)
route_id (FK)
capacity
operator_name

3. arrival_logs
log_id (PK)
bus_id (FK)
stop_name
scheduled_time
actual_time
date
weather

4. feedback
feedback_id (PK)
bus_id (FK)
rating
comments

structure:
public-transport-reliability-sql/
├── README.md
├── tablesinfo.txt               # Table creation queries
├── transport analysis.txt       # Analysis SQL queries
├── data_csv/
    ├── buses.csv
    ├── routes.csv
    ├── arrival_logs.csv
    └── feedback.csv
