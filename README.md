# 🏨 Hospitality Revenue Analytics  
### Power BI Dashboard | CodeBasics Project

A comprehensive Power BI analytics solution designed to provide actionable insights to the Revenue Team in the Hospitality Domain. This project analyzes booking patterns, revenue metrics, and operational performance across multiple hotel properties.

---

## 📊 Project Overview

This analytics dashboard helps hospitality businesses understand their revenue performance, booking trends, and operational efficiency through interactive visualizations and key performance indicators.

---

## 🔍 Business Objective

- Track revenue generated vs revenue realized
- Analyze booking patterns and cancellations
- Improve occupancy and capacity utilization
- Compare property and room category performance
- Identify customer behavior and satisfaction trends

---

## 🧱 Data Model

The project follows a **Star Schema** data model for optimized analytics performance.

---

## 📁 Dataset Structure

### ⭐ Dimension Tables

#### 📅 dim_date.csv
| Column | Description |
|------|------------|
| date | Dates spanning May, June, and July |
| mmm yy | Month-year format (e.g., May 25) |
| week no | Unique week number |
| day_type | Weekend or Weekday |

#### 🏨 dim_hotels.csv
| Column | Description |
|------|------------|
| property_id | Unique hotel identifier |
| property_name | Name of the hotel |
| category | Luxury or Business |
| city | Hotel location |

#### 🛏️ dim_rooms.csv
| Column | Description |
|------|------------|
| room_id | RT1, RT2, RT3, RT4 |
| room_class | Standard, Elite, Premium, Presidential |

---

### 📌 Fact Tables

#### 📈 fact_aggregated_bookings.csv
| Column | Description |
|------|------------|
| property_id | Hotel identifier |
| check_in_date | Check-in date |
| room_category | Room type |
| successful_bookings | Number of successful bookings |
| capacity | Maximum available rooms |

#### 🧾 fact_bookings.csv
| Column | Description |
|------|------------|
| booking_id | Unique booking identifier |
| property_id | Hotel identifier |
| booking_date | Date of booking |
| check_in_date | Customer check-in date |
| check_out_date | Customer check-out date |
| no_guests | Number of guests |
| room_category | Room type |
| booking_platform | Booking channel |
| ratings_given | Customer ratings |
| booking_status | Cancelled, Checked Out, No Show |
| revenue_generated | Total booking revenue |
| revenue_realized | Actual revenue (40% deduction on cancellations) |

---

## 📈 Analytics Capabilities

- Revenue trend analysis
- Occupancy rate calculation
- Booking platform performance comparison
- Cancellation and no-show analysis
- Weekend vs weekday performance
- Property-wise and category-wise insights
- Customer satisfaction analysis

---

## 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- CSV Data Sources
- Star Schema Data Model

---

## 📂 Files in Repository

```
├── dim_date.csv                          # Date dimension table
├── dim_hotels.csv                        # Hotels dimension table
├── dim_rooms.csv                         # Rooms dimension table
├── fact_aggregated_bookings.csv          # Aggregated bookings data
├── fact_bookings.csv                     # Detailed bookings data
├── meta_data_hospitality.txt             # Data dictionary
├── Problem_Statement_and_Tasks.docx      # Project requirements
└── Hospitality-Revenue-Analytics.pbix    # Power BI report file
```

---

## 🚀 Getting Started

### Prerequisites
- Microsoft Power BI Desktop (Latest Version)

2. **Installation**
   - Clone this repository
   ```bash
   git clone https://github.com/VAISHNAVPS07/Hospitality_Revenue_Analytics_PowerBI.git
   ```

3. **Open the Dashboard**
   - Launch Power BI Desktop
   - Open `Hospitality-Revenue-Analytics.pbix`
   - Explore the interactive visualizations

## 📊 Data Dictionary

Complete metadata and column descriptions are available in `meta_data_hospitality.txt`

## 👤 Authors

- **Vaishnav P S**
- **Sriram K**
- **Samarth M**
- **Suhaas D**



*Built with Power BI for Hospitality Revenue Analytics*
