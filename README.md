# Delivery Performance Intelligence

<div align="center">

![Hero Banner](https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0f172a,100:2563eb&text=E-commerce%20Logistics%20Analytics&fontColor=ffffff&fontSize=34&animation=fadeIn&fontAlignY=38)

![Typing](https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=18&duration=2200&pause=900&color=38BDF8&center=true&vCenter=true&width=900&lines=8%2C577+Raw+Rows+%E2%86%92+8%2C449+Cleaned+Rows;Exact+metrics+computed+from+repository+files;Operations+insight+for+speed%2C+quality%2C+and+scale)

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Analytics](https://img.shields.io/badge/Analytics-0A66C2?style=for-the-badge&logo=databricks&logoColor=white)
![Dashboard](https://img.shields.io/badge/Dashboard-FF6F00?style=for-the-badge&logo=googleanalytics&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

</div>

---

## Mission

This capstone transforms e-commerce shipment records into operational intelligence for courier performance, service-level behavior, and city-level delivery reliability.

Core decision question:
**Which delivery levers improve speed without compromising customer experience?**

---

## Exact Data Snapshot (File-Verified)

All numbers below were computed directly from:
- `Rawdataset/Dataset_ecommerce - Raw_Data.csv`
- `Cleaned/Dataset_ecommerce - cleaned.csv`

| Metric | Value |
|---|---:|
| Raw records | 8,577 |
| Cleaned records | 8,449 |
| Removed/resolved rows | 128 |
| Courier partners | 5 |
| Cities | 20 |
| Districts | 329 |
| Avg estimated delivery time | 2.814 days |
| Avg product rating | 2.996 / 5 |
| Date range | 2022-06-11 to 2023-06-11 |

---

## Pipeline

```mermaid
flowchart LR
    A[Raw Data<br/>8,577 rows] --> B[Cleaning + Standardization]
    B --> C[Cleaned Data<br/>8,449 rows]
    C --> D[Pivot Metrics]
    D --> E[Dashboard Layer]
    E --> F[Business Insights]
```

---

## Courier Benchmark (Exact)

```mermaid
xychart-beta
    title "Avg Estimated Delivery Time by Courier (days)"
    x-axis ["Ninja Xpress","Jne","Sicepat","J&T Express","Pos Indonesia"]
    y-axis "Days" 2.70 --> 2.90
    bar [2.729,2.803,2.826,2.843,2.869]
```

```mermaid
pie showData
    title Courier Order Share
    "Sicepat (1,745)" : 1745
    "Pos Indonesia (1,715)" : 1715
    "Jne (1,671)" : 1671
    "Ninja Xpress (1,665)" : 1665
    "J&T Express (1,653)" : 1653
```

| Courier | Orders | Avg Days | Avg Rating |
|---|---:|---:|---:|
| Ninja Xpress | 1,665 | 2.729 | 2.968 |
| Jne | 1,671 | 2.803 | 2.981 |
| Sicepat | 1,745 | 2.826 | 3.006 |
| J&T Express | 1,653 | 2.843 | 2.995 |
| Pos Indonesia | 1,715 | 2.869 | 3.026 |

---

## Delivery-Type Performance (Exact)

```mermaid
xychart-beta
    title "Avg Estimated Delivery Time by Delivery Type (days)"
    x-axis ["Express","Next Day","Reguler","Same Day"]
    y-axis "Days" 2.70 --> 2.90
    bar [2.742,2.814,2.843,2.859]
```

| Delivery Type | Orders | Avg Days |
|---|---:|---:|
| Express | 2,145 | 2.742 |
| Next Day | 2,031 | 2.814 |
| Reguler | 2,125 | 2.843 |
| Same Day | 2,148 | 2.859 |

---

## City-Level Contrast (Only Cities >= 150 Orders)

### Fastest Cities
- Malang: **2.611** days (435 orders)
- Surakarta: **2.657** days (411 orders)
- Makassar: **2.686** days (440 orders)
- Tangerang: **2.702** days (440 orders)
- Yogyakarta: **2.705** days (431 orders)

### Slowest Cities
- Semarang: **2.971** days (409 orders)
- Depok: **2.953** days (443 orders)
- Bandung: **2.931** days (423 orders)
- Bogor: **2.927** days (410 orders)
- Surabaya: **2.916** days (430 orders)

---

## Business Insights

- Delivery performance gap between couriers exists, but it is relatively tight.
- `Ninja Xpress` is fastest by average delivery days.
- `Pos Indonesia` has the highest average product rating.
- Service label and speed are not perfectly aligned in this data (`Same Day` is slowest on average).
- City-level differences indicate local operational bottlenecks/opportunities.

---

## Repository Map

```text
DVA-Capstone/
├── Rawdataset/
│   └── Dataset_ecommerce - Raw_Data.csv
├── Cleaned/
│   └── Dataset_ecommerce - cleaned.csv
├── Calculations_Pivots/
│   └── Dataset_ecommerce - cleaned - Pivot Table.csv
├── dashboard/
│   ├── Dataset_ecommerce - cleaned - Dashboard.csv
│   ├── Dataset_ecommerce - cleaned - Dashboard.pdf
│   └── dashboard.png
├── Documentation/
│   ├── Delivery_Performance_Analysis.pdf
│   └── Report.pdf
└── README.md
```

---

## Data Dictionary

| Field | Description |
|---|---|
| `product_id` | Product/order ID |
| `order_date` | Order date (`DD/MM/YY`) |
| `courier_delivery` | Courier partner |
| `city` | Destination city |
| `district` | Destination district |
| `type_of_delivery` | Service level (`Express`, `Next Day`, `Reguler`, `Same Day`) |
| `estimated_delivery_time_days` | Estimated shipping duration in days |
| `product_rating` | Customer rating (1-5) |

---

## Dashboard Contents

- KPI cards (orders, avg delivery time, avg rating)
- Courier speed comparison
- Delivery-type comparison
- Courier order-share split
- City performance ranking
- Filter-driven exploratory view

---

## Team

**Group 4 | Section A**
# Delivery Performance Intelligence

<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&height=180&color=0:0ea5e9,100:6366f1&text=E-commerce%20Logistics%20Analytics&fontColor=ffffff&fontSize=36&animation=fadeIn&fontAlignY=35)

![Typing SVG](https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=18&duration=2600&pause=900&color=0EA5E9&center=true&vCenter=true&width=900&lines=Raw+Data+%E2%86%92+Cleaned+Data+%E2%86%92+Business+Insight;8%2C577+rows+profiled+%7C+8%2C449+rows+analyzed;Speed%2C+Reliability%2C+Customer+Experience)

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-0A66C2?style=for-the-badge&logo=databricks&logoColor=white)
![Dashboard](https://img.shields.io/badge/Dashboard-FF6F00?style=for-the-badge&logo=googleanalytics&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

</div>

---

## Project Focus

This capstone evaluates e-commerce delivery performance across Indonesia using courier, geography, and delivery-type dimensions.

Primary question:
**Which operational levers improve delivery speed while maintaining customer satisfaction?**

---

## Exact Dataset Snapshot

Numbers below are computed directly from files in this repository (`Rawdataset` + `Cleaned`):

- Raw records: **8,577**
- Cleaned records: **8,449**
- Rows removed/resolved during cleaning: **128**
- Courier partners: **5**
- Cities: **20**
- Districts: **329**
- Average estimated delivery time: **2.814 days**
- Average product rating: **2.996 / 5**
- Date range in cleaned file: **11/06/2022 to 11/06/2023**

---

## Data-to-Insight Pipeline

```mermaid
flowchart LR
    A[Raw CSV<br/>8,577 rows] --> B[Cleaning & Standardization]
    B --> C[Cleaned Dataset<br/>8,449 rows]
    C --> D[Pivot Calculations]
    D --> E[Dashboard Assets]
    E --> F[Operational Insights]
```

---

## Courier Performance (Exact)

```mermaid
xychart-beta
    title "Average Estimated Delivery Time by Courier (days)"
    x-axis ["Ninja Xpress","Jne","Sicepat","J&T Express","Pos Indonesia"]
    y-axis "Days" 2.65 --> 2.9
    bar [2.729,2.803,2.826,2.843,2.869]
```

```mermaid
pie showData
    title Courier Order Mix (8,449 orders)
    "Sicepat (1,745)" : 1745
    "Pos Indonesia (1,715)" : 1715
    "Jne (1,671)" : 1671
    "Ninja Xpress (1,665)" : 1665
    "J&T Express (1,653)" : 1653
```

Courier summary table:

| Courier | Orders | Avg Delivery Days | Avg Rating |
|---|---:|---:|---:|
| Ninja Xpress | 1,665 | 2.729 | 2.968 |
| Jne | 1,671 | 2.803 | 2.981 |
| Sicepat | 1,745 | 2.826 | 3.006 |
| J&T Express | 1,653 | 2.843 | 2.995 |
| Pos Indonesia | 1,715 | 2.869 | 3.026 |

---

## Delivery-Type Analysis (Exact)

```mermaid
xychart-beta
    title "Average Estimated Delivery Time by Delivery Type (days)"
    x-axis ["Express","Next Day","Reguler","Same Day"]
    y-axis "Days" 2.7 --> 2.9
    bar [2.742,2.814,2.843,2.859]
```

| Delivery Type | Orders | Avg Delivery Days |
|---|---:|---:|
| Express | 2,145 | 2.742 |
| Next Day | 2,031 | 2.814 |
| Reguler | 2,125 | 2.843 |
| Same Day | 2,148 | 2.859 |

---

## Geography Contrast (Cities with 150+ Orders)

Fastest:
- Malang (**2.611**, 435 orders)
- Surakarta (**2.657**, 411 orders)
- Makassar (**2.686**, 440 orders)
- Tangerang (**2.702**, 440 orders)
- Yogyakarta (**2.705**, 431 orders)

Slowest:
- Semarang (**2.971**, 409 orders)
- Depok (**2.953**, 443 orders)
- Bandung (**2.931**, 423 orders)
- Bogor (**2.927**, 410 orders)
- Surabaya (**2.916**, 430 orders)

---

## Key Business Insights

- Delivery-time differences across couriers are measurable but narrow.
- `Ninja Xpress` leads on speed; `Pos Indonesia` leads slightly on average rating.
- Service labels do not perfectly map to speed expectations (`Same Day` appears slowest in this dataset).
- City-level operations likely explain a meaningful share of variability.

---

## Repository Structure

```text
DVA-Capstone/
├── Rawdataset/
│   └── Dataset_ecommerce - Raw_Data.csv
├── Cleaned/
│   └── Dataset_ecommerce - cleaned.csv
├── Calculations_Pivots/
│   └── Dataset_ecommerce - cleaned - Pivot Table.csv
├── dashboard/
│   ├── Dataset_ecommerce - cleaned - Dashboard.csv
│   ├── Dataset_ecommerce - cleaned - Dashboard.pdf
│   └── dashboard.png
├── Documentation/
│   ├── Delivery_Performance_Analysis.pdf
│   └── Report.pdf
└── README.md
```

---

## Data Dictionary

| Field | Description |
|---|---|
| `product_id` | Product/order identifier |
| `order_date` | Order placement date (`DD/MM/YY`) |
| `courier_delivery` | Courier partner name |
| `city` | Delivery city |
| `district` | Delivery district |
| `type_of_delivery` | Service tier (`Express`, `Next Day`, `Reguler`, `Same Day`) |
| `estimated_delivery_time_days` | Estimated shipment duration in days |
| `product_rating` | Customer product rating from 1 to 5 |

---

## Dashboard Components

- KPI cards (total orders, avg delivery time, avg rating)
- Courier speed comparison
- Delivery type vs speed view
- Courier share distribution
- City performance ranking
- Interactive slicer-based filtering

---

## Team

**Group 4 | Section A**
# Delivery Performance Intelligence

<div align="center">

### E-commerce Logistics Analytics Capstone

From raw shipment data to a recruiter-ready operations intelligence story.

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-0A66C2?style=for-the-badge&logo=databricks&logoColor=white)
![Dashboarding](https://img.shields.io/badge/Dashboard-FF6F00?style=for-the-badge&logo=googleanalytics&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

</div>

---

## Why This Project Stands Out

This project analyzes courier delivery behavior across Indonesia and transforms a noisy dataset into business-ready operational insight.  
It focuses on speed, reliability, and customer satisfaction to answer a key logistics question:

**Which delivery levers actually improve customer experience at scale?**

---

## Executive Snapshot

- **8,577** raw records profiled
- **8,449** cleaned records retained (**128 rows resolved/removed**)
- **5 couriers**, **20 cities**, **329 districts**
- **Average estimated delivery time:** `2.814 days`
- **Average product rating:** `2.996 / 5`
- **Data period:** `2022-01-07` to `2023-12-05`

---

## Tech Stack

<div align="center">

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=flat-square&logo=googlesheets&logoColor=white)
![Google Drive](https://img.shields.io/badge/Google_Drive-4285F4?style=flat-square&logo=googledrive&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-00C4CC?style=flat-square&logo=canva&logoColor=white)

</div>

---

## Data Pipeline

```mermaid
flowchart LR
    A[Raw CSV Dataset<br/>8,577 rows] --> B[Data Cleaning]
    B --> C[Standardization]
    C --> D[Pivot Calculations]
    D --> E[Dashboard Build]
    E --> F[Business Insights]
```

---

## What Was Cleaned

- Removed duplicate/irrelevant records
- Standardized categorical labels (`courier_delivery`, `city`, `district`)
- Normalized `estimated_delivery_time_days` into numeric form
- Reshaped date values for consistent timeline analysis
- Prepared pivot-ready data for dashboard KPIs and charts

---

## Performance Insights

### 1) Courier Speed Benchmark (lower is better)

```mermaid
xychart-beta
    title "Avg Estimated Delivery Time by Courier (days)"
    x-axis ["Ninja Xpress","Jne","Sicepat","J&T Express","Pos Indonesia"]
    y-axis "Days" 2.6 --> 2.95
    bar [2.729,2.803,2.826,2.843,2.869]
```

**Takeaway:** `Ninja Xpress` is the fastest performer, while `Pos Indonesia` is the slowest by average delivery duration.

### 2) Delivery Type Behavior

```mermaid
xychart-beta
    title "Avg Delivery Time by Delivery Type (days)"
    x-axis ["Express","Next Day","Reguler","Same Day"]
    y-axis "Days" 2.7 --> 2.9
    bar [2.742,2.814,2.843,2.859]
```

**Takeaway:** `Express` is fastest; `Same Day` appears slowest in this dataset, signaling possible process or labeling nuances.

### 3) Order Share by Courier

```mermaid
pie showData
    title Courier Order Mix (8,449 orders)
    "Sicepat (1,745)" : 1745
    "Pos Indonesia (1,715)" : 1715
    "Jne (1,671)" : 1671
    "Ninja Xpress (1,665)" : 1665
    "J&T Express (1,653)" : 1653
```

**Takeaway:** Workload is evenly distributed; no single courier dominates volume.

### 4) City-Level Delivery Contrast

- **Fastest large cities (150+ orders):**
  - Malang (`2.611`)
  - Surakarta (`2.657`)
  - Makassar (`2.686`)
  - Tangerang (`2.702`)
  - Yogyakarta (`2.705`)

- **Slowest large cities (150+ orders):**
  - Semarang (`2.971`)
  - Depok (`2.953`)
  - Bandung (`2.931`)
  - Bogor (`2.927`)
  - Surabaya (`2.916`)

---

## Business Interpretation

- Courier-level speed differences are measurable but relatively narrow
- Service-tier labels do not always map to expected speed outcomes
- Geographic segmentation matters: city-level operations likely drive significant variance
- Product ratings are stable across couriers, suggesting service speed is not the only CX driver

---

## Repository Structure

```text
DVA-Capstone/
├── Rawdataset/
│   └── Dataset_ecommerce - Raw_Data.csv
├── Cleaned/
│   └── Dataset_ecommerce - cleaned.csv
├── Calculations_Pivots/
│   └── Dataset_ecommerce - cleaned - Pivot Table.csv
├── dashboard/
│   └── Dataset_ecommerce - cleaned - Dashboard.csv
└── readme.md
```

---

## Data Dictionary

| Field | Description |
|---|---|
| `product_id` | Product/order identifier |
| `order_date` | Date order was placed |
| `courier_delivery` | Courier partner |
| `city` | Delivery city |
| `district` | Delivery district |
| `type_of_delivery` | Service level (Express, Next Day, Reguler, Same Day) |
| `estimated_delivery_time_days` | Estimated shipment duration in days |
| `product_rating` | Customer rating (1 to 5) |

---

## Dashboard Features

- KPI cards: total orders, avg delivery time, avg rating
- Courier-level delivery comparison
- Delivery type vs speed comparison
- Courier order-share donut
- City performance ranking
- Slicers for courier, delivery type, and city analysis

---

## Recruiter Quick Pitch

This capstone demonstrates end-to-end analytics execution:
- data cleaning discipline,
- metric design,
- visual storytelling,
- and operational insight extraction from real-world logistics data.

It reflects the practical mindset expected in Data Analyst, Business Analyst, and Operations Analytics roles.

---

## Team

**Group 4 | Section A**
# Delivery Performance Intelligence

<div align="center">

### E-commerce Logistics Analytics Capstone

From raw shipment data to a recruiter-ready operations intelligence story.

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-0A66C2?style=for-the-badge&logo=databricks&logoColor=white)
![Dashboarding](https://img.shields.io/badge/Dashboard-FF6F00?style=for-the-badge&logo=googleanalytics&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

</div>

---

## Why This Project Stands Out

This project analyzes courier delivery behavior across Indonesia and transforms a noisy dataset into business-ready operational insight.  
It focuses on speed, reliability, and customer satisfaction to answer a key logistics question:

**Which delivery levers actually improve customer experience at scale?**

---

## Executive Snapshot

- **8,577** raw records profiled
- **8,449** cleaned records retained (**128 rows resolved/removed**)
- **5 couriers**, **20 cities**, **329 districts**
- **Average estimated delivery time:** `2.814 days`
- **Average product rating:** `2.996 / 5`
- **Data period:** `2022-01-07` to `2023-12-05`

---

## Tech Stack

<div align="center">

![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=flat-square&logo=googlesheets&logoColor=white)
![Google Drive](https://img.shields.io/badge/Google_Drive-4285F4?style=flat-square&logo=googledrive&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-00C4CC?style=flat-square&logo=canva&logoColor=white)

</div>

---

## Data Pipeline

```mermaid
flowchart LR
    A[Raw CSV Dataset<br/>8,577 rows] --> B[Data Cleaning]
    B --> C[Standardization]
    C --> D[Pivot Calculations]
    D --> E[Dashboard Build]
    E --> F[Business Insights]
```

---

## What Was Cleaned

- Removed duplicate/irrelevant records
- Standardized categorical labels (`courier_delivery`, `city`, `district`)
- Normalized `estimated_delivery_time_days` into numeric form
- Reshaped date values for consistent timeline analysis
- Prepared pivot-ready data for dashboard KPIs and charts

---

## Performance Insights

### 1) Courier Speed Benchmark (lower is better)

```mermaid
xychart-beta
    title "Avg Estimated Delivery Time by Courier (days)"
    x-axis ["Ninja Xpress","Jne","Sicepat","J&T Express","Pos Indonesia"]
    y-axis "Days" 2.6 --> 2.95
    bar [2.729,2.803,2.826,2.843,2.869]
```

**Takeaway:** `Ninja Xpress` is the fastest performer, while `Pos Indonesia` is the slowest by average delivery duration.

### 2) Delivery Type Behavior

```mermaid
xychart-beta
    title "Avg Delivery Time by Delivery Type (days)"
    x-axis ["Express","Next Day","Reguler","Same Day"]
    y-axis "Days" 2.7 --> 2.9
    bar [2.742,2.814,2.843,2.859]
```

**Takeaway:** `Express` is fastest; `Same Day` appears slowest in this dataset, signaling possible process or labeling nuances.

### 3) Order Share by Courier

```mermaid
pie showData
    title Courier Order Mix (8,449 orders)
    "Sicepat (1,745)" : 1745
    "Pos Indonesia (1,715)" : 1715
    "Jne (1,671)" : 1671
    "Ninja Xpress (1,665)" : 1665
    "J&T Express (1,653)" : 1653
```

**Takeaway:** Workload is evenly distributed; no single courier dominates volume.

### 4) City-Level Delivery Contrast

- **Fastest large cities (150+ orders):**
  - Malang (`2.611`)
  - Surakarta (`2.657`)
  - Makassar (`2.686`)
  - Tangerang (`2.702`)
  - Yogyakarta (`2.705`)

- **Slowest large cities (150+ orders):**
  - Semarang (`2.971`)
  - Depok (`2.953`)
  - Bandung (`2.931`)
  - Bogor (`2.927`)
  - Surabaya (`2.916`)

---

## Business Interpretation

- Courier-level speed differences are measurable but relatively narrow
- Service-tier labels do not always map to expected speed outcomes
- Geographic segmentation matters: city-level operations likely drive significant variance
- Product ratings are stable across couriers, suggesting service speed is not the only CX driver

---

## Repository Structure

```text
DVA-Capstone/
├── Rawdataset/
│   └── Dataset_ecommerce - Raw_Data.csv
├── Cleaned/
│   └── Dataset_ecommerce - cleaned.csv
├── Calculations_Pivots/
│   └── Dataset_ecommerce - cleaned - Pivot Table.csv
├── dashboard/
│   └── Dataset_ecommerce - cleaned - Dashboard.csv
└── readme.md
```

---

## Data Dictionary

| Field | Description |
|---|---|
| `product_id` | Product/order identifier |
| `order_date` | Date order was placed |
| `courier_delivery` | Courier partner |
| `city` | Delivery city |
| `district` | Delivery district |
| `type_of_delivery` | Service level (Express, Next Day, Reguler, Same Day) |
| `estimated_delivery_time_days` | Estimated shipment duration in days |
| `product_rating` | Customer rating (1 to 5) |

---

## Dashboard Features

- KPI cards: total orders, avg delivery time, avg rating
- Courier-level delivery comparison
- Delivery type vs speed comparison
- Courier order-share donut
- City performance ranking
- Slicers for courier, delivery type, and city analysis

---

## Recruiter Quick Pitch

This capstone demonstrates end-to-end analytics execution:
- data cleaning discipline,
- metric design,
- visual storytelling,
- and operational insight extraction from real-world logistics data.

It reflects the practical mindset expected in Data Analyst, Business Analyst, and Operations Analytics roles.

---

## Team

**Group 4 | Section A**