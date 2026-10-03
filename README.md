# 🚀 Global Space Launch Analytics & Superpower Reliability (1957–2020)

[![Tableau Public](https://img.shields.io/badge/Tableau%20Public-Interactive%20Dashboard-E97627?logo=tableau&logoColor=white)](https://public.tableau.com/views/SpaceMissionsViz_17908789981330/Orbital_Launch_Dashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Express%20%26%20Graph%20Objects-3F4F75?logo=plotly&logoColor=white)](https://plotly.com/)

An end-to-end exploratory data analysis and business intelligence project tracking humanity's access to orbit over 63 years. This study models historical launch cadence, financial expenditure profiles, engineering failure curves, and the geopolitical transition from the Cold War duopoly to modern multipolar commercialization.

---

## 📊 Live Interactive Dashboard

Explore the interactive dashboard on **Tableau Public**:  
👉 **[View Live Dashboard: Global Space Launch Cadence & Vehicle Reliability](https://public.tableau.com/views/SpaceMissionsViz_17908789981330/Orbital_Launch_Dashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**

### Dashboard Architecture
* **Executive KPI Summary:** Live aggregate tracking of global volume ($4,198$ missions through 2020), overall mission success rate ($90.4\%$), and cumulative vehicle losses ($404$ anomalies).
* **Geopolitical Market Share (100% Stacked Bar):** Year-by-year distribution visualizing the shift from Soviet/US dominance to the entrance of Europe, China, India, and commercial space.
* **Flight Reliability & Vehicle Attrition Tracker (Dual-Axis):** Direct juxtaposition of raw annual failure counts against the systemic failure rate percentage ($1957–2020$).
* **Space Power Reliability Matrix (Decade Highlight Table):** Decade-by-decade operational maturity across major space blocs (USA, USSR/Russia, China, Europe, India, Japan, and Rest of World).

---

## 🔍 Key Analytical Findings

### 1. The Aerospace Learning Curve & The 1995 Inflection Point
* **The "Infant Mortality" Era (1957–1962):** Early orbital testing suffered failure rates between **30% and 55%** due to acoustic combustion instabilities, microgravity restart failures, and early analog avionics.
* **Structural Stabilization Post-1995:** Failure rates permanently stabilized **below 10%** (averaging $4\%–6\%$ from 2000 onward). This shift was driven by triple-redundant digital flight computers, consolidation around proven "heritage" booster architectures (Soyuz, Delta II, Long March), and commercial satellite insurance requirements.

### 2. Space Economics & Cost Tiers
Analysis of disclosed launch budgets ($N = 964$ missions with published financial figures) revealed an inverse relationship between budget scale and mission failure:
* **Tier 1 — Small-Sat / Budget (< $20M):** **74.2% Success Rate** (Experimental micro-launchers, maiden flight qualification attrition).
* **Tier 2 — Commercial Workhorses ($20M – $100M):** **93.4% Success Rate** (Mass-produced medium/heavy boosters like Falcon 9, Long March 2/3, PSLV).
* **Tier 3 — Heavy Lifters & Human Spaceflight (> $100M):** **97.8% Success Rate** (Mission-critical state architectures including the Space Shuttle, Saturn V, and ULA Atlas/Delta IV).

### 3. Geopolitical Shifts: Duopoly to Multipolarity
* **Cold War Era (1957–1991):** The United States and Soviet Union held a virtual duopoly, with the USSR sustaining peak rates of 80–100 launches annually during the 1970s and 1980s.
* **Commercial Emergence (1990s–2000s):** Europe (Arianespace) captured over 50% of the commercial geostationary telecommunications launch market.
* **Modern Era (2010s–2020):** China's CASC scaled rapidly, conducting 30–40 launches annually and briefly surpassing US annual cadence before SpaceX's commercial reusability ramped to scale.

---

## ⚠️ Data Lineage & Sampling Limitation Note

> **Catalog Omission Bias (1992–2015 Russian Records):**  
> While Cold War coverage (1957–1991) and modern records (2016–2020) are comprehensive, granular inspection of the scraped dataset revealed severe sampling omission for Russian missions launched from Baikonur Cosmodrome between 1992 and 2015. Recorded launches drop from an average of ~55/year pre-1991 to ~2.6/year during this window. This reflects an upstream catalog scraping artifact rather than actual orbital dormancy. All post-1991 superpower cadence comparisons in the dashboard are annotated with this domain context.

---

## 🛠️ Data Pipeline & Engineering Workflow
