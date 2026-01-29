# 🏨 Revenue Insights in the Hospitality Domain
### Provides insights using KPI's, Charts, Measures and others on the hospitality data.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)

## 📌 Project Overview
This project focuses on analyzing **revenue performance, occupancy trends, booking behavior, and customer ratings** in the hospitality industry using **Power BI**.

The objective is to help hotel management:
- Identify revenue leakage
- Improve occupancy rates
- Optimize pricing and room utilization
- Track booking platform performance
- Make data-driven strategic decisions

The dashboard is built using a **star schema data model** with fact and dimension tables and industry-standard KPIs.


## 🎯 Business Objectives
- Track **Total Revenue, ADR, RevPAR, Occupancy %**
- Compare **Luxury vs Business hotels**
- Analyze **city-wise and hotel-wise performance**
- Understand **booking platform contribution**
- Monitor **weekend vs weekday trends**
- Identify **cancellations and no-show impact**


## 🧰 Tools & Technologies Used
- **Power BI** – Data modeling, DAX, dashboarding
- **Microsoft Excel** – Data validation & metrics reference
- **CSV Files** – Raw dataset
- **DAX** – KPI calculations
- **GitHub** – Project versioning & documentation


## 📂 Dataset Description
The project uses **5 CSV files** following a star schema structure :contentReference[oaicite:0]{index=0}

### 🔹 Dimension Tables

#### `dim_date`
| Column | Description |
|------|------------|
| date | Calendar date |
| mmm yy | Month-Year format |
| week no | Unique week number |
| day_type | Weekday / Weekend |

#### `dim_hotels`
| Column | Description |
|------|------------|
| property_id | Unique hotel ID |
| property_name | Hotel name |
| category | Luxury / Business |
| city | Hotel location |

#### `dim_rooms`
| Column | Description |
|------|------------|
| room_id | Room type (RT1–RT4) |
| room_class | Standard, Elite, Premium, Presidential |


### 🔹 Fact Tables

#### `fact_bookings`
| Column | Description |
|------|------------|
| booking_id | Unique booking ID |
| property_id | Hotel ID |
| booking_date | Booking date |
| check_in_date | Check-in date |
| check_out_date | Check-out date |
| no_guests | Number of guests |
| room_category | Room type |
| booking_platform | Booking channel |
| ratings_given | Customer rating |
| booking_status | Cancelled / Checked Out / No Show |
| revenue_generated | Total booking revenue |
| revenue_realized | Final revenue after adjustments |

#### `fact_aggregated_bookings`
| Column | Description |
|------|------------|
| property_id | Hotel ID |
| check_in_date | Check-in date |
| room_category | Room type |
| successful_bookings | Confirmed bookings |
| capacity | Available rooms |


## 🧮 Key KPIs & Metrics
- **Total Revenue**
- **Revenue Realized**
- **Occupancy %**
- **Average Daily Rate (ADR)**
- **Revenue per Available Room (RevPAR)**
- **Cancellation Rate**
- **No Show Rate**
- **Average Rating**
- **Booking Platform Contribution**

All KPIs are calculated using **DAX measures** following hospitality industry standards.


## 📊 Dashboard Pages
1. **Executive Overview**
   - Revenue, Occupancy %, RevPAR, ADR
   - Trend analysis

2. **Hotel Performance Analysis**
   - City-wise & hotel-wise revenue
   - Luxury vs Business comparison

3. **Booking Insights**
   - Platform-wise bookings
   - Cancellation & no-show impact

4. **Time-Based Analysis**
   - Weekly trends
   - Weekend vs Weekday performance


## 🧠 Key Insights Generated
- Luxury hotels generate higher ADR but lower occupancy compared to Business hotels
- Weekends show higher occupancy but increased cancellation rates
- Certain booking platforms contribute high volume but lower realized revenue
- City-wise performance varies significantly, highlighting expansion opportunities


## 📁 Project Structure
```
📦 Revenue-Insights-Hospitality
┣ 📂 data
┃ ┣ dim_date.csv
┃ ┣ dim_hotels.csv
┃ ┣ dim_rooms.csv
┃ ┣ fact_bookings.csv
┃ ┗ fact_aggregated_bookings.csv
┣ 📂 dashboard
┃ ┗ Revenue-Insights-in-the-Hospitality-Domain.pbix
┣ 📂 reference
┃ ┣ metrics-list.xlsx
┃ ┗ meta_data_hospitality.txt
┗ README.md
```


## 🚀 How to Use This Project
1. Clone the repository
2. Open the `.pbix` file in **Power BI Desktop**
3. Refresh data connections if required
4. Explore interactive visuals and filters


## 💼 Resume Bullet (You Can Use This)
Built an end-to-end **Hospitality Revenue Insights Dashboard** using Power BI, analyzing occupancy, ADR, RevPAR, booking behavior, and cancellation impact across multiple cities and hotel categories using DAX and star schema modeling.


## 📄 Licence
This project is licensed under the MIT License — see the LICENSE file for details.


## 👤 Author
**K Keerthi**  
Data Science Engineering Student <br>
Aspiring Python Developer / Data Analyst
 

⭐ If you find this project helpful, feel free to star the repository!

---

<p align="center">
  🛠 Built by <a href="https://github.com/KEERTHI2355">@Keerthi2355</a> 
  <br>
  <a href="#-the-vault">Back to Top</a>
</p>


