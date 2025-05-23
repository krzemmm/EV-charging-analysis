# ⚡ **EV Charging Habits Analysis**

## 📘 Project Overview

This project focuses on analyzing **shared electric vehicle (EV) charging stations** in residential apartment buildings. The aim is to understand how these shared resources are used by tenants — including patterns of use, peak hours, and user behaviors that may affect charger availability. Insights from this analysis help property managers optimize infrastructure planning and ensure equitable access to chargers.

## 🎯 Objectives

* Analyze usage trends for **shared charging stations only** (excluding private ones).
* Identify **peak demand times** and usage frequency by day and hour.
* Detect **charging behavior patterns** such as long session durations and high-usage garages.
* Provide **data-driven recommendations** to improve access, fairness, and tenant satisfaction.

## 🛠️ Tools & Technologies

| Tool / Language                      | Purpose                                |
| ------------------------------------ | -------------------------------------- |
| PostgreSQL                           | Data querying and aggregation          |
| Python (pandas, seaborn, matplotlib) | Data manipulation and visualizations   |
| Jupyter Notebook                     | Interactive analysis and reporting     |

## 🧮 Dataset

**Table:** `charging_sessions`
Key columns:

* `garage_id`, `user_id`, `user_type`, `start_plugin`, `end_plugout`
* `start_plugin_hour`, `duration_hours`, `el_kwh`, `month_plugin`, `weekdays_plugin`

**Note:** All analyses are **filtered for shared stations only** (`user_type = 'Shared'`).

**Source:** [Kaggle – Residential EV Charging](https://www.kaggle.com/datasets/anshtanwar/residential-ev-chargingfrom-apartment-buildings)

## 📈 Key Analysis (Shared Stations Only)

### 👥 Unique Users per Garage

Analyzes how many unique tenants used shared charging stations in each garage, helping identify high-demand buildings.

### ⏰ Most Popular Charging Start Times

Identifies the most frequent start times for shared charging sessions, revealing daily usage peaks and pressure points.

### 🕒 Long-Duration Shared Users

Highlights users with an average session duration over 10 hours, indicating potential overuse or misuse of shared infrastructure.

### 📅 Average Sessions Per Day by Weekday

Explores how shared station usage varies throughout the week, showing which days have the highest and lowest average session counts.

### 🔥 Peak Demand Hours (Heatmap)

Generates a heatmap showing session volumes across all hours and days of the week for shared stations. This visualization helps building managers understand temporal demand patterns and optimize scheduling or infrastructure placement.

## 📂 Project Files

* Full notebook with SQL queries and visualizations
* Excel initial data
