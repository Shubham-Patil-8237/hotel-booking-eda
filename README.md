# 🏨 Hotel Booking Analysis – Exploratory Data Analysis (EDA)

This project performs a comprehensive Exploratory Data Analysis (EDA) on a real-world hotel booking dataset to uncover key insights about guest behavior, pricing (ADR), booking trends, cancellations, and operational efficiency.

---

## 📌 Problem Statement

**Uncovering Patterns in Hotel Booking Data for Operational Efficiency and Revenue Growth**

The goal is to analyze historical hotel booking records and identify:
- Revenue-driving factors like market segment and special requests
- Trends in cancellations and booking lead times
- Guest demographics, group size behavior, and nationality distribution
- Operational inefficiencies like room reassignments (upgrades)

---

## 📂 Dataset Details

- **Source**: `hotel_bookings.csv`
- **Rows**: 119,390
- **Columns**: 32
- **Key Features**:
  - `adr`: Average Daily Rate
  - `lead_time`: Days between booking and check-in
  - `is_canceled`: Whether booking was cancelled
  - `customer_type`, `market_segment`, `distribution_channel`
  - `reserved_room_type`, `assigned_room_type`
  - `total_of_special_requests`, `booking_changes`, `country`

---

## 🛠 Technologies Used

- Python 3.13
- Pandas & NumPy for data processing
- Seaborn & Matplotlib for visualization
- SciPy for statistical testing
- Jupyter Notebook for development

---

## 📊 Key Steps

### 1. Data Cleaning
- Handled missing values (`company`, `agent`, `children`, `country`)
- Converted object columns to `category` type
- Created datetime column `arrival_date`
- Derived columns: `total_stay`, `total_guests`, `is_upgraded`

### 2. Exploratory Data Analysis (EDA)
- **Univariate**: Histograms & countplots
- **Bivariate**: Boxplots of ADR vs market_segment, customer_type
- **Time-Series**: Monthly trends, country-wise booking patterns
- **Correlation Matrix**: Heatmap and numeric correlation

### 3. Hypothesis Testing
- 2-Sample T-Test: Online TA vs Direct (ADR)
- Chi-Square Test: Lead time vs room upgrades
- ANOVA: Stay duration across customer types

### 4. Business Questions Answered
- What influences ADR the most?
- Are guests with early bookings more likely to change/cancel?
- Do different countries behave differently?
- Which segments bring more revenue or cancellations?
- How often are rooms upgraded or reassigned?

---

## 🔍 Insights

- **Special requests and upgrades correlate with higher ADR**
- **Transient and corporate guests contribute more to revenue**
- **Guests from Spain and France tend to pay higher ADR**
- **Room upgrades occur in ~12.5% of bookings**
- **Online TA has the highest cancellation rate**

---

## ✅ Conclusion

This project successfully reveals operational and revenue-impacting patterns in hotel bookings using EDA and hypothesis testing. The insights can help optimize pricing, forecast cancellations, and improve guest experience.

---

## 📁 Files

- `hotel_bookings.csv` – Input dataset
- `EDA_hotel_bookings.csv.ipynb` – Jupyter Notebook (all code + charts)
- `Hotel_Booking_EDA_Report.docx` – Final formatted report
- `README.md` – Project overview

---

## 🙋‍♂️ Author

**Shubham Sanjay Patil**  
CDAC Kharghar | PG-DBDA 2025  
[GitHub](https://github.com/) | [LinkedIn](linkedin.com/in/shubhampatilmca)

---
