# Movie Rental Store Analysis  
**Power BI • Excel EDA • SQL • Business Intelligence**

---

## Project Overview
This project presents a **comprehensive business intelligence and analytics solution** for a DVD rental store using the **Sakila Movie Rental Database**. The analysis focuses on understanding **customer behavior, rental trends, film performance, inventory efficiency, staff and store operations, geographic demand patterns, and actor influence**.

The primary objective is to support **data-driven decision-making** by transforming raw transactional data into **actionable insights** through structured **Excel-based exploratory data analysis (EDA)** and **interactive Power BI dashboards**. The project is designed as a full-cycle analytics workflow, from raw data ingestion to executive-ready reporting.

A **MECE (Mutually Exclusive, Collectively Exhaustive)** analytical framework is applied throughout the project to ensure clarity, completeness, and non-overlapping insights.

---

## Business Objectives
- Understand **revenue drivers and seasonality**
- Segment customers and analyze **loyalty behavior**
- Evaluate **film, category, and actor performance**
- Optimize **inventory and replacement cost management**
- Assess **rental behavior and return patterns**
- Analyze **geographic and store-level performance**
- Enable **strategic planning and marketing decisions**

---

## Data Model & Architecture
The analysis is built on **15+ normalized relational tables**, covering the entire operational lifecycle of a movie rental business.

### Core Entities
- Customers, Rentals, Payments  
- Films, Categories, Actors  
- Inventory, Stores, Staff  
- Address, City, Country, Language  

### Key Relationships
- **Many-to-many**: film ↔ actor, film ↔ category  
- **One-to-many**: customer → rental → payment  
- **Inventory-based rentals** mapped across stores and locations  

An **Entity Relationship (ER) Diagram** is included in the repository to visually represent table relationships and data flow.

---

## Methodology & Workflow

### 1️ Data Acquisition
- Raw data sourced from the Sakila DVD Rental dataset
- CSV files imported for analysis and modeling

### 2️ Data Cleaning & Preparation
- Handled missing values, duplicates, and inconsistencies
- Standardized categorical fields and date formats
- Verified relational integrity across tables

### 3️ Exploratory Data Analysis (EDA)
- Performed **EDA in Microsoft Excel** using pivot tables, charts, and aggregations
- Answered structured business problem statements related to customers, revenue, rentals, inventory, and geography
- Identified trends, anomalies, and correlations for further analysis

### 4️ SQL-Based Analysis
- Used SQL joins and aggregations to extract analytical datasets
- Addressed complex business questions across multiple tables
- Prepared structured outputs for Excel and Power BI consumption

### 5️ Power BI Visualization
- Built a **multi-page interactive Power BI dashboard**
- Created KPIs, slicers, drill-downs, and cross-filtered visuals
- Translated analytical findings into clear business narratives

---

## Key KPIs & Insights

### Revenue & Seasonality
- **67.4K total revenue** from **16K+ rental transactions**
- **July identified as the peak revenue month**
- **Sports and Sci-Fi** emerged as the highest revenue-generating categories

### Customer & Loyalty Analysis
- Analyzed **599 customers across 20+ countries**
- Identified **97.5% active customers**
- Strong positive relationship between **customer loyalty and revenue**
- Detected onboarding gaps among new customers with zero purchases

### Rental Behavior
- Majority of rentals returned within **3–7 days**
- Early and late return patterns impact inventory turnover
- Rental frequency increases significantly with **store proximity**

### Film, Inventory & Actor Performance
- Higher rental-rate films consistently showed higher demand
- High replacement-cost films still generated strong revenue
- **PG-13 and NC-17** ratings dominated customer demand
- Actor “star power” measurably influenced rental volume

### Geographic & Store Insights
- Category demand varied significantly by city and country
- **Action and Sports** categories dominated multiple locations
- Store location played a critical role in customer engagement

---

## Tools & Technologies
- **Microsoft Excel** – Exploratory Data Analysis (EDA)  
- **SQL (MySQL)** – Data extraction, joins, aggregations  
- **Power BI** – Interactive dashboards and KPI reporting  
- **GitHub** – Version control and documentation  

---

## Repository Structure
```text
Movie-Rental-Store-Analysis/
│
├── assets/
│   ├── overview.png
│   ├── revenue_examination.png
│   ├── customer_insights.png
│   ├── film_performance_analysis.png
│   ├── geographic_analysis.png
│   ├── actor_analysis.png
│   ├── top_rentals.png
│   └── er_diagram.png
│
├── data/
│   ├── csv/
│   │   ├── actor.csv
│   │   ├── address.csv
│   │   ├── category.csv
│   │   ├── city.csv
│   │   ├── country.csv
│   │   ├── customer.csv
│   │   ├── film.csv
│   │   ├── film_actor.csv
│   │   ├── film_category.csv
│   │   └── film_text.csv
│   │
│   └── sql/
│       └── movie_rental_queries.sql
│
├── docs/
│   ├── data_dictionary.pdf
│   └── dvd_rental_store_insights.pdf
│
├── excel/
│   └── movie_rental_analysis_EDA.xlsx
│
├── powerBI/
│   ├── movie_rental_analysis.pbix
│   ├── analytical_powerBI_report.pdf
│   └── er_diagram.png
│
└── README.md
