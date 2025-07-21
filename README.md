# 🛡️ Security & Personnel Services Dashboard  -> Market Strategy and client Development tracker
**Business Analytics Portfolio – Excel 2016**

## 📁 Overview  
This project demonstrates a strategic dashboard built for a fictional security services provider. The Excel-based model simulates client data, operational metrics, compliance tracking, and business development insights — showcasing real-world analyst skills using mock data and interactive visuals.

---

## 🧪 Data Preparation

**1. Data Source**  
- Generated using Python and Pandas (200 records)  
- Covers sectors like **Construction, Retail, Industrial, Corporate, Residential**

**2. Table Conversion & Formatting**  
- Cleaned headers and converted to Excel Table (`Ctrl + T`)  
- Currency formatted as ₹ INR, percentages styled clearly  
- Applied data validation lists for fields like `Sector`, `Location`, and `Compliance_Flag`

**3. Conditional Formatting Highlights**  
- `Certification Valid (%) < 65%` → 🔴 undertrained flag  
- `SLA Breaches > 2` → 🟠 service quality risk

**4. Calculated Columns for Enriched Analysis**  
```excel
Revenue_per_guard           =IF([@Guard_Count]=0, 0, [@Monthly_Deal_Value]/[@Guard_Count])  
Incident_Rate_per_Guard     =IF([@Guard_Count]=0, 0, [@Incident_Reports]/[@Guard_Count])  
Pitch_Efficiency            =IF([@[Pitch_Success (%)]]>=80,"High", IF([@[Pitch_Success (%)]]>=60,"Moderate","Low"))
```

---

## 📊 Dashboard Features & Insights

1. **Lead Status Funnel**  
   - 52% clients converted, 32% pitch ongoing, 15% cold leads  
   ➤ Reflects strong acquisition and sales pipeline

2. **Sector Revenue**  
   - Corporate sector leads in revenue, followed by Residential  
   ➤ Identifies most valuable industries

3. **Compliance Distribution**  
   - High-risk clients concentrated in Thane; Borivali shows strong compliance  
   ➤ Regional focus for quality audits or training updates

4. **SLA Breaches by Sector & Location**  
   - Construction clients in Thane and Navi Mumbai breach service agreements most  
   ➤ Operational bottlenecks or resource gaps

5. **Pitch Efficiency Score**  
   - 52% of clients rated “Low”  
   ➤ Suggests strategic review of proposals and engagement tactics

6. **Incident Pattern**  
   - 50+ clients reported ≥2 incidents with avg. Incident Rate per Guard ≈ 6  
   ➤ High workload or undertraining correlation observed

7. **Certification vs Incident Correlation (Scatter Plot)**  
   - Clients served by highly certified guards tend to report fewer incidents  
   ➤ Visual proof of training ROI



