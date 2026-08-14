# Swiggy Data Intelligence Platform

> **End-to-end Azure Data Engineering & Power BI Analytics Platform for Food Delivery Intelligence**

## 📌 Project Overview

This project is an end-to-end data intelligence platform built to simulate how a food delivery business can collect, process, store, transform, and analyze operational data at scale.

The primary objective was not just to build a Power BI dashboard, but to understand and implement a complete **cloud-based data engineering workflow using Microsoft Azure**, followed by business intelligence and analytical reporting.

The platform combines:

- ☁️ Azure cloud services
- 🔄 Automated data pipelines
- 🗄️ Cloud-based data storage and database systems
- 🧹 Data transformation and preparation
- 📊 Power BI analytics
- 💡 Business insights and recommendations

---

## 🏗️ Solution Architecture

The project follows an end-to-end data flow:

**Source Data → Azure Data Storage → Azure Data Factory → Cloud Database → Power BI → Business Intelligence**

The pipeline was designed to separate data ingestion, storage, transformation, and visualization into distinct stages.

### Data Engineering Layer

- **Azure Data Factory** — Pipeline orchestration and data movement
- **Azure Storage** — Cloud-based data storage
- **Azure Database** — Structured storage and querying of processed data

### Analytics Layer

- **Power BI** — Data modeling, DAX calculations, interactive dashboards, and business analysis

---

## 🔄 Data Pipeline

The Azure pipeline follows a structured ETL/ELT workflow:

1. Ingest source food-delivery datasets
2. Store raw data in Azure
3. Move and process data through Azure Data Factory
4. Load structured data into the cloud database
5. Build analytical relationships and measures
6. Connect Power BI to the processed data
7. Develop interactive business dashboards
8. Translate analytical findings into business recommendations

This workflow helped me understand how cloud data platforms connect the **engineering layer with the business intelligence layer**.

---

## 📊 Power BI Dashboard

The Power BI report contains **7 analytical pages**, each designed around a specific business perspective.

### 1. Executive Overview

Provides a high-level view of overall business performance including:

- Total orders
- Revenue
- Average delivery time
- Delivery rating
- Average order value
- Monthly order and revenue performance
- Restaurant revenue performance
- Order status distribution
- Executive business insights

![Executive Overview](screenshots/Executive%20Overview.png)

---

### 2. Customer Analytics

Focuses on customer behaviour, frequency, and value.

Key analysis includes:

- Customer order frequency
- Repeat customers
- Repeat rate
- Customer value segmentation
- Top customers by revenue
- Customer rating
- Order frequency vs customer revenue

![Customer Analytics](screenshots/Customer%20Analytics.png)

---

### 3. Restaurant Analytics

Analyzes restaurant performance and customer experience.

Key analysis includes:

- Top restaurants by revenue
- Restaurant revenue by city
- Revenue by cuisine
- Average restaurant rating
- Restaurant rating vs revenue
- Restaurant-level performance comparison

![Restaurant Analytics](screenshots/Restaurant%20Analytics.png)

---

### 4. Delivery Analytics

Examines delivery performance and operational efficiency.

Key analysis includes:

- Delivery time by hour
- Delivery time vs distance
- Delivery performance by traffic and weather
- Order status distribution
- Delivery delay drivers

![Delivery Analytics](screenshots/Delivery%20Analytics.png)

---

### 5. Orders Analytics

Provides transaction-level analysis of order behaviour.

Key analysis includes:

- Order activity over time
- Order value distribution
- Order status journey
- Discount vs order value
- Coupon usage mix
- Cancellation rate
- Average discount per order

![Orders Analytics](screenshots/Order%20Analytics.png)

---

### 6. Deep Dive

An interactive investigation page designed for root-cause analysis.

Users can investigate delivery performance using combinations of:

- Traffic level
- Weather
- Cuisine
- Delivery city
- Restaurant
- Individual orders

The page combines interactive filters, decomposition analysis, restaurant-level performance, and order-level investigation.

![Deep Dive](screenshots/Deep%20Dive.png)

---

### 7. Insights & Actions

The final page converts the analysis into actionable business recommendations.

Key findings include:

- Delivery risk hotspots
- Core order-value range
- Coupon usage behaviour
- Cancellation risk
- Recommended operational and commercial actions

![Insights & Actions](screenshots/Insights%20&%20Actions.png)

---

## 💡 Key Business Insights

### 🚚 Delivery Performance

High traffic and rainy weather are associated with significantly higher delivery times, with certain city and vehicle combinations creating noticeable operational bottlenecks.

### 💰 Order Value

A large proportion of orders fall within the **₹200–₹600** range, creating an opportunity to increase basket size through bundles, add-ons, and targeted recommendations.

### 🎟️ Coupon Usage

Approximately **35% of orders use coupons**, suggesting that promotions have a meaningful role in customer purchasing behaviour.

### ⚠️ Cancellation Risk

Approximately **8.78% of orders are cancelled**, representing an opportunity to investigate cancellation drivers and reduce avoidable revenue leakage.

### 👥 Customer Behaviour

The customer analysis highlights repeat purchasing patterns and allows high-value customers to be separated from lower-value segments.

---

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| Cloud Platform | Microsoft Azure |
| Data Orchestration | Azure Data Factory |
| Cloud Storage | Azure Storage |
| Database | Azure Cloud Database |
| Data Transformation | SQL / Azure Data Services |
| Business Intelligence | Power BI |
| Data Modeling | Power BI / DAX |
| Version Control | GitHub |

---

## 📁 Repository Structure

```text
swiggy-data-intelligence-platform/
│
├── screenshots/
│   ├── Executive Overview.png
│   ├── Customer Analytics.png
│   ├── Restaurant Analytics.png
│   ├── Delivery Analytics.png
│   ├── Order Analytics.png
│   ├── Deep Dive.png
│   └── Insights & Actions.png
│
├── powerbi/
│   └── Swiggy_Data_Intelligence_Platform.pbix
│
└── README.md
