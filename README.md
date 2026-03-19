<img width="1438" height="818" alt="Screenshot 2026-03-19 at 11 35 24 PM" src="https://github.com/user-attachments/assets/12e37235-c8a7-4b87-b116-8b6ecd8586b9" />
# 🏥 Hospital Management Dashboard

## 📌 Dashboard Goal
Provide a clear, visual summary of patient admissions, doctor performance, billing, and treatment trends to help management monitor hospital efficiency and financial health.

This Tableau dashboard provides a single visual view of hospital operations, helping management monitor:
- Patient flow  
- Doctor performance  
- Revenue generation  
- Treatment efficiency  

It converts raw hospital data into actionable insights to support quick, data-driven decisions across departments like administration, finance, and medical management.

---

## 🎯 Target
The dashboard helps hospital leaders make faster, data-driven decisions about:
- Patient care  
- Doctor performance  
- Financial health  

➡️ Improving both service quality and profitability.

---

## 📊 KPIs

| KPI Name | Description | Formula (Tableau) |
|----------|------------|-------------------|
| Total Patients | Count of all unique patients | `COUNTD([PatientID])` |
| Average Feedback Rating | Average of patient feedback ratings | `AVG([FeedbackRating])` |
| Total Revenue Collected | Sum of all AmountPaid | `SUM([AmountPaid])` |
| Pending Amount | Total pending payments | `SUM([PendingAmount])` |

---

## 📊 Bar Charts

| Chart Name | Purpose | Dimensions & Measures |
|------------|--------|-----------------------|
| Patients by City | Identify cities with most patients | City vs `COUNT(PatientID)` |
| Doctor-wise Total Billing | Identify high-performing doctors | DoctorName vs `SUM(TotalBillAmount)` |
| Disease-wise Patient Count | Common diseases treated | Disease vs `COUNT(PatientID)` |
| Department-wise Revenue | Department earnings comparison | Department vs `SUM(AmountPaid)` |

---

## 📈 Line Charts

| Chart Name | Purpose | Details |
|------------|--------|---------|
| Monthly Admissions Trend | Admissions over time | AdmissionDate (month) vs `COUNT(PatientID)` |
| Monthly Billing Trend | Revenue trend per month | BillingDate (month) vs `SUM(AmountPaid)` |
| Follow-up Trends | Track patient follow-ups | FollowUpDate (month) vs `COUNT(PatientID)` |

---

## 🍩 Donut Charts

| Chart Name | Purpose | Details |
|------------|--------|---------|
| Surgery Required % | Ratio of patients requiring surgery | % of SurgeryRequired = 'Yes' |
| Payment Mode Split | Show how patients pay | PaymentMode vs `COUNT(PatientID)` |

---

## 🌳 Tree Map

| Chart Name | Purpose | Details |
|------------|--------|---------|
| Revenue by State and City | Identify high revenue regions | State (hierarchy) vs `SUM(AmountPaid)` |

---

## ⭐ Top 5 Bar Chart

| Chart Name | Purpose | Details |
|------------|--------|---------|
| Top 5 Doctors by Feedback Rating | Identify top-rated doctors | DoctorName vs `AVG(FeedbackRating)` (Top 5 only) |

---

## 🧩 Dashboard Layout Suggestion

- **Top Row:** 4 KPI cards  
- **Second Row:** 2 bar charts  
  - Patients by City  
  - Doctor-wise Billing  
- **Third Row:** 2 bar charts  
  - Disease Count  
  - Department Revenue  
- **Fourth Row:** 3 line charts  
  - Admissions  
  - Billing  
  - Follow-ups  
- **Fifth Row:** 2 donut charts  
  - Surgery %  
  - Payment Mode  
- **Bottom Row:**  
  - Tree Map  
  - Top 5 Doctors bar chart  

---

## ✅ Expected Outcome

- Identify top-performing doctors and departments  
- Track revenue and pending payments  
- Analyze trends in admissions, billing, and follow-ups  
- Improve hospital efficiency and decision-making  

---

## 📎 Source
Based on Hospital Dashboard PDF  
https://public.tableau.com/app/profile/sudhanshu.shekhar6644/viz/Hospital_17739433170240/Dashboard1?publish=yes
