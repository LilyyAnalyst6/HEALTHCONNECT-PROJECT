HealthConnect Clinic — Data Analytics Track

AnalystLab Africa Experience Lab | HealthConnect Clinic Experience Lab

Reducing missed appointments and improving patient support at a fictional healthcare clinic, using exploratory data analysis, KPI development, statistical validation, and an interactive Power BI dashboard.

Project question: How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?

📁 Repository Contents
File	Description
HealthConnect_Appointment_Data_cleaned.csv	Week 5 cleaned dataset (missing values imputed, grouping columns added)
HealthConnect_Appointment_Data_cleaned_v2.csv	Week 6 dataset — adds the refined 4-factor risk_v2 column
HealthConnect_Week6_DataAnalytics_Report.docx	Week 6: statistical validation, deeper analysis, refined risk model, cross-track integration
HealthConnect_Dashboard.pbix	Power BI dashboard (3 pages — see below)

📊 Dashboard Overview

Page 1 — Executive Overview Headline KPIs (Total Appointments, Attended, Cancelled, No-Shows, Overall No-Show Rate, Repeat No-Show Rate) alongside the primary drivers: distance band, reminder status, booking lead time, and prior no-show history — each with a reminder-status breakdown for interaction context.

Page 2 — Secondary Drivers Day of week, time of day, reminder channel, appointment type, and the original 3-factor risk segmentation (Low/Medium/High Risk), with synced slicers carried over from Page 1.

Page 3 — Validated Findings & Refined Risk Segments (Week 6) A validation table confirming which Week 5 factors are statistically significant, the refined 4-factor risk segment (Critical/Medium/Minimal Risk), a live Critical Risk Count, and a lead-time-by-distance interaction chart.

🔑 Key Findings
Finding	Result
Overall no-show rate	51.2% (n = 4,737 eligible appointments)
Strongest validated driver	Booking lead time — 29.5% (0–7 days) → 71.4% (45+ days)
Repeat no-show rate	57.8% (has prior no-show) vs. 46.3% (clean record)
Distance effect	48.7% (<5km) → 56.9% (>15km)
Reminder effect	54.6% (no reminder) → 49.9% (reminder sent); SMS performs best
Refined risk segment (Week 6)	Critical Risk: 80.9% vs. Minimal Risk: 22.4% — a validated 58.5-point spread

Day of week, time of day, age group, and gender were tested and found not statistically significant — they are not used as targeting criteria.

🧪 Methodology
Week 5: Data quality assessment → EDA → 5 KPIs → dashboard → 6 business insights
Week 6: Chi-square significance testing of every Week 5 factor → multivariate logistic regression to confirm independent effects → refined 4-factor risk segmentation validated with 95% confidence intervals → dashboard extended (not rebuilt) → findings handed off to the Data Science track as candidate model features

Full methodology, statistical results, and business recommendations are documented in the two .docx reports.

🤝 Cross-Track Integration

Findings and the risk_v2 feature were shared with the Data Science track as validated, ranked candidate inputs for their no-show prediction model — replacing an untested list of correlations with a statistically confirmed feature ranking (lead time > prior no-shows > distance > reminders).

⚠️ Limitations
Dataset is fictional/simulated and does not reflect real-world clinical behaviour
Cancelled appointments are excluded from the no-show rate denominator (pending formal business confirmation)
Critical/Minimal risk segments are based on ~100 appointments each; directionally reliable but should be re-validated as more data becomes available
🛠 Tools Used


Power BI for the interactive dashboard · Microsoft Word for reporting# HEALTHCONNECT-PROJECT
