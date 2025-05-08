# 📊 AtliQ Grands: Data-Driven Strategies to Optimize Hotel Revenue and Market Share

## 📑 Table of Contents
1. [Project Overview]  
2. [Business Problem]  
3. [Data Overview] 
4. [Approach]  
   - [Data Acquisition & Cleaning]  
   - [Data Modeling]  
   - [DAX Calculations]  
   - [Dashboard Development] 
5. [Key Insights Uncovered]  
6. [Recommendations]  
7. [Conclusion]

---

## 📘 Project Overview
**AtliQ Grands**, a leading chain of luxury and business hotels in India, faced significant challenges, including a decline in **market share** and **revenue**. Increased competition, a lack of **data-backed decision-making**, and the absence of an **internal analytics team** led to the underutilization of historical data, resulting in missed strategic opportunities.

To address these challenges, an interactive and comprehensive **Power BI dashboard** was developed, transforming raw booking data into **actionable insights**. These insights aimed to **optimize revenue**, enhance **pricing strategies**, and improve overall **business performance** in a highly competitive market.


*The screenshots provided below highlight the Power BI dashboards created for AtliQ Grands, enabling data-driven insights for improved business performance.*



![Dashboard1](https://github.com/user-attachments/assets/d0283758-1119-4882-a8cc-863ac2ee3975)




![Dashbord 2](https://github.com/user-attachments/assets/e41ee944-cd6b-490b-882c-dc79dff9116d)


---

## ❓ Business Problem
Despite being a prominent brand in the **luxury hospitality segment**, AtliQ Grands faced several setbacks, including:

- Shrinking **market share** due to stronger **competitor strategies**
- Declining **revenues** from key city hotels
- Lack of **data-driven decision-making** processes
- Absence of **internal analytics infrastructure** to extract value from available booking data

The core objective of this project was to extract valuable insights from the company’s past booking data to:

- Analyze **customer behavior** and **booking patterns**
- Monitor and improve **operational KPIs**
- Recommend **tailored strategies** to improve **occupancy**, **revenue**, and overall **hotel performance**

---

## 📁 Data Overview
**Time Frame**: May–July 2022 (Week 18–31; Week 32 excluded for accuracy)  
**Hotel Portfolio**: 7 Hotels (4 Luxury, 3 Business) across Mumbai, Bengaluru, Hyderabad, and Delhi  
### Data Model:
- **Fact Tables**: `Fact_Bookings`, `FactAggregated_Bookings`  
- **Dimension Tables**: `Dim_Date`, `Dim_Rooms`, `Dim_Hotels`
### Key Columns for Analysis: Revenue, Room Class, Booking Platform, Occupancy, Booking Status, Guest Count


---

### Tools and Technologies Used:

| Tool/Technology | Purpose |
|-----------------|---------|
| **Excel** | Initial data exploration, validation, and pre-analysis |
| **Power Query** | Data cleaning, transformation, and shaping |
| **DAX** | Creating custom KPIs, measures, and logic-based metrics |
| **Power BI** | Visual report and dashboard creation |

---

## 🛠️ Approach
The project was delivered through a **four-phase analytics lifecycle**:

### 1. Data Acquisition & Cleaning
- Imported and examined fact and dimension tables
- Verified data quality using Power BI’s **Column Quality** tool—confirmed **absence of nulls**
- Standardized **data types** across numeric, categorical, and date fields
- Corrected **header alignment issues** in `Dim_Rooms` for structural consistency
- Enriched the `Dim_Date` table with two calculated columns:
  - **Week number** for temporal trend analysis  
  - **Day type (Weekday/Weekend)** for behavioral segmentation  

### 2. Data Modeling
- Implemented a **Star Schema** to optimize performance and enable **drill-down analysis**
- Created **one-to-many relationships** between fact and dimension tables
- Ensured proper **relationship cardinality** and **filter directions** for intuitive reporting

### 3. DAX Calculations
Developed key performance metrics:

- **Revenue KPIs**: Total Revenue, ADR, RevPAR  
- **Booking KPIs**: Total Bookings, DURN, DBRN, DSRN  
- **Efficiency Metrics**: Occupancy Rate, Realization %, Cancellation Rate  

### 4. Dashboard Development
Two interactive **Power BI dashboards** were created to offer comprehensive insights:

#### Dashboard 1 – Hotel Overview (Executive Insights)
- **KPI Cards**: Total Revenue, Total Bookings, Occupancy Rate, Cancellation Rate, Avg. Rating  
- **Visuals**:
  - Revenue by State/Hotel – Bar chart with drill-down  
  - Weekday vs Weekend Analysis – Decomposition Tree  
  - Platform-wise Bookings – Funnel chart  
  - Booking Status – Pie chart  
  - Room Class-wise Revenue – Donut chart  
- **Slicers**: Hotel Category, Month  
- **Navigation**: Link to revenue and occupancy performance dashboard

#### Dashboard 2 – Revenue and Occupancy Performance Dashboard
- **KPI Cards**: ADR, RevPAR, Realization %, DURN, DBRN, DSRN  
- **Line Charts**: WoW % change in Revenue, RevPAR, ADR, etc.  
- **Slicers**: Month, Hotel Category, State, Hotel Name  

---

## 📈 Key Insights Uncovered
- **Revenue & Occupancy Patterns**:  
  May showed peak performance with the highest revenue, RevPAR, and occupancy (**overall occupancy = 58%**), indicating potential for further optimization during low seasons.

- **Booking Platform Insights**:  
  The “Others” platform delivered the highest **RevPAR (₹3001)**, while **Direct Offline underperformed (₹371)**.  
  Strong opportunities identified on **MakeMyTrip** and **Others** to drive revenue growth.

- **Regional Hotel Performance**:
  - **Mumbai**: Highest contributor to total revenue. A key city for premium customer targeting.  
  - **Bengaluru**: Moderate revenue but lowest average rating (**3.4**), signaling issues in customer satisfaction or service delivery.  
  - **Hyderabad & Delhi**: Consistent performance with untapped potential for both **business** and **luxury segments**.

- **Room Type Analysis**:
  - **Presidential and Premium Rooms** generated more revenue and catered to larger groups.  
  - **Elite Rooms** favored by smaller groups – ideal for couples or solo travelers.  
  - Opportunity to apply **targeted promotions** based on group size and room type preference.

- **Cancellation & No-Show Rates**:
  - **Cancellation Rate**: 25%  
  - **No-Show Rate**: 5%  
  Substantial revenue loss identified, warranting a review of current **confirmation and cancellation policies**.

---

## 💡 Recommendations
Based on in-depth analysis, the following strategies were proposed to maximize revenue and improve operational performance:

- **Cancellation Reduction**  
  Implement flexible yet firm cancellation and confirmation policies, leveraging **email/SMS reminders** and **loyalty incentives** to reduce churn.

- **ADR Improvement via Upselling**  
  Promote **premium services** (spa, dining, extended stays) and encourage **room upgrades** during booking confirmation.

- **City-Specific Strategies**:
  - **Mumbai**: Expand premium offerings to meet high-end demand  
  - **Bengaluru**: Improve service delivery and guest satisfaction  
  - **Hyderabad**: Capitalize on strong ratings in the business travel segment  
  - **Delhi**: Focus on luxury segment differentiation and personalized offerings  

- **Boost Weekday Bookings**  
  Design **loyalty points systems** and **weekday-only corporate packages**.

- **Dynamic Weekend Pricing**  
  Offer strategic **discounts during off-peak weekends** without lowering RevPAR.

- **Strengthen OTA and Direct Channels**  
  Encourage **direct bookings** via web campaigns and maintain visibility and performance on top-performing OTAs like **MakeMyTrip**.

- **Reduce No-Shows & Improve Check-Outs**  
  Incentivize **early check-outs** with discounts or perks and implement **automated check-in reminders and confirmations**.

- **Room-Type Targeting**  
  Use **customer segmentation** to market presidential rooms to groups and premium rooms to families or business travelers.

---

## ✅ Conclusion
The **Power BI dashboard** empowered **AtliQ Grands** with **data-backed insights** across **revenue**, **bookings**, **occupancy**, **customer behavior**, and **platform/channel effectiveness**. These insights laid the foundation for **actionable strategies** that can:

- Boost **ADR**, **RevPAR**, and **occupancy**
- Reduce **cancellations** and **no-shows**
- Enhance **customer satisfaction**
- Target **city-level opportunities**
- Improve **platform ROI** and **room-type sales**

By integrating **descriptive**, **diagnostic**, and **strategic analytics** into a centralized dashboard, this project demonstrated how **data can be transformed into meaningful business action**—bridging the gap between **information and impact**.

