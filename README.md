# E-commerce Hybrid Migration Project (MySQL → MongoDB)

## 🚀 Overview
This project demonstrates hybrid database migration:
- Migrate transactional data (users/orders) from MySQL to MongoDB.
- Store new feature data (analytics, preferences) directly in MongoDB.

## 📁 Project Structure
- `etl_scripts/` — Scripts to migrate users and orders.
- `validation/` — Script to verify record counts.
- `monitoring/` — Docker stack for Prometheus + Grafana.

## 🔧 Setup
1. Start MySQL and MongoDB locally.
2. Run `migrate_users.py` and `migrate_orders.py` from `etl_scripts/`.
3. Validate using `validate_row_counts.py`.
4. Launch monitoring with `docker-compose up -d`.

## 🛠 Requirements
- Python 3, PyMySQL, PyMongo
- Docker, Docker Compose
- MongoDB Exporter (for Prometheus metrics)
  
