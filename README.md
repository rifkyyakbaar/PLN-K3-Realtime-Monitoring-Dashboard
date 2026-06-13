# PLN-K3-Realtime-Monitoring-Dashboard

**Author:** Rifky Akbar Utomo Putra  
**Role:** Software Developer  

---

## About The Project
This project is a web-based **Real-time Monitoring Dashboard** developed for the Occupational Health and Safety (K3) Division at PT PLN Indonesia Power UBP Jeranjang. It transforms massive raw face recognition log data into interactive visual analytics. 

The system utilizes a custom First-In Last-Out (FILO) algorithm to accurately filter duplicate attendance entries caused by high personnel mobility. Built with an asynchronous fetching architecture, the dashboard provides continuous live updates without page reloads, ensuring rapid data access for emergency response readiness.

## Disclaimer: Dummy Data Usage
Please note that the database and records provided in this repository contain **100% synthetic/dummy data**. 

PT PLN Indonesia Power UBP Jeranjang is a designated National Vital Object (*Objek Vital Nasional/Obvitnas*). Due to strict corporate security policies and data privacy regulations, the original production database—which contains real-time biometric tracking logs of actual employees cannot be published online. 

The dummy data (generated via Laravel Seeders/Factories) is included solely to demonstrate how the system's logic, FILO algorithm, Smart Calendar Heatmap, and data visualizations function in a simulated environment.

## Key Features
* **Real-time Capacity Tracking:** Live monitoring of personnel inside the operational zone without requiring manual page refresh.
* **FILO Algorithm:** Automatically processes raw, duplicate entry/exit logs to calculate effective working hours accurately.
* **Smart Calendar Heatmap:** Visualizes daily attendance patterns and anomalies using intuitive color-coded indicators.
* **Dynamic Filtering:** Filter data easily by specific zones, dates, or departments.
* **Automated Excel Export:** Extract clean, filtered data into formatted `.xlsx` reports for administrative needs.
* **Direct Access (Kiosk Mode):** Designed to operate on closed Intranet networks without session timeouts for 24/7 monitoring.

## Tech Stack
* **Backend:** Laravel 10 (PHP)
* **Frontend:** Bootstrap 5, Vanilla JavaScript, HTML/CSS
* **Database:** PostgreSQL
* **Others:** AJAX (Asynchronous JavaScript and XML)

---

## 💻 Installation Guide

Follow these steps to install and run the project on your local machine:

### Prerequisites
* PHP >= 8.1
* Composer
* PostgreSQL installed and running
* Git

### Step-by-Step Installation
## 💻 Installation Guide

Follow these steps to install and run the project on your local machine. Ensure you have **PHP >= 8.1**, **Composer**, **PostgreSQL**, and **Git** installed before proceeding.

### Step-by-Step Installation

```bash
# 1. Clone the repository and navigate into the project directory
git clone [https://github.com/yourusername/your-repo-name.git](https://github.com/yourusername/your-repo-name.git)
cd your-repo-name

# 2. Install all required PHP dependencies via Composer
composer install

# 3. Create your local environment configuration file
cp .env.example .env

# 4. Configure your database settings
# Open the .env file in your code editor and update the PostgreSQL credentials:
# DB_CONNECTION=pgsql
# DB_HOST=127.0.0.1
# DB_PORT=5432
# DB_DATABASE=your_local_database_name
# DB_USERNAME=your_postgres_username
# DB_PASSWORD=your_postgres_password

# 5. Generate a unique application security key
php artisan key:generate

# 6. Run migrations and seeders 
# (CRITICAL: This generates the tables and populates the synthetic/dummy data)
php artisan migrate --seed

# 7. Start the local development server
php artisan serve
```
---
## ✨ Thank You!
Thanks for checking out this repository! I hope this project gives you a clear picture of my approach to building practical and efficient web systems. Feel free to explore the code, and don't hesitate to reach out if you have any questions or feedback. Enjoy!

Enjoy exploring the code and the system!
