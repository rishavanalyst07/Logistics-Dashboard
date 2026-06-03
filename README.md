# Logistics-Dashboard


1. 📌 Project Overview
This project involved building an end-to-end Logistics Analytics Dashboard in Power BI to monitor and track order fulfillment performance across a supply chain. The core problem was that the logistics team lacked real-time visibility into delivery statuses, SLA (Service Level Agreement) breaches, RTO (Return to Origin) trends, and TAT (Turnaround Time) — leading to delayed decisions and poor customer experience. The dashboard solved this by centralizing all logistics KPIs into a single interactive view, covering a date range across multiple weeks (e.g., Oct 24 – Dec 3, 2025).

2. 🧑‍💻 Your Role & Contribution

Solely or primarily responsible for requirement gathering from the logistics/ops team
Designed the data model and report layout from scratch
Wrote DAX measures for KPIs like SLA%, RTO%, TAT averages, and split-by-day calculations
Built all visuals: pie charts, line charts, TAT tables, and order-level drill-through tables
Delivered the final report for business stakeholder review and daily operational use


3. 🗄️ Data Sources & Tools
LayerToolRaw DataExcel files from logistics/ops teams (order data, pickup dates, delivery status)Storage/QueryingSQL Server Management Studio (SSMS) / Azure SQL Database for structured storageTransformationPower Query (ETL inside Power BI) + possibly Azure Data Factory for pipelineVisualizationMicrosoft Power BI (Desktop + Service)ConnectivityDirectQuery or Import mode connecting Power BI to Azure/SSMS

4. ⚙️ Process / Methodology

Data Collection — Gathered raw order/shipment data from Excel and operational systems
Data Ingestion — Loaded into SQL Server (SSMS/Azure) for structured querying
Data Cleaning & Transformation — Used Power Query to handle nulls, date formatting, status mapping
Data Modeling — Built a star schema with Orders as fact table, dates/cities/status as dimensions
DAX Development — Created measures for SLA%, RTO count, TAT (O2D, O2S, S2D), and rolling day splits (T-7, T-14)
Visualization — Designed the dashboard layout with KPI cards, pie charts, trend lines, and reference number lookup
Testing & Validation — Cross-verified numbers with source Excel files with the ops team
Deployment — Published to Power BI Service for daily stakeholder access


5. ✨ Key Features of the Solution

KPI Summary Bar — Orders, Delivered, Pending, In-Transit, Cancelled, RTO, Orders Within TAT at a glance
TAT Tracking — Three TAT breakdowns: O2D (Order to Delivery), O2S (Order to Shipment), S2D (Shipment to Delivery) with daily trend tables
SLA Status (Closed & Open Cases) — Separate pie charts showing SLA breach rate for closed vs. open orders (~91% closed within TAT, ~84% open within TAT)
Delivery Within SLA by Day — Line chart tracking daily SLA% fluctuations over weeks
RTO Split by Days — T-14, T-7, and Today breakdowns to monitor return trends over time
Reference No. Lookup — Search bar to drill into individual order details (city, pickup date, transit flag, delivery status)
Dynamic Date Filter — Slicer to filter the entire dashboard by order date range


6. 📈 Impact & Results

Reduced time to identify SLA breaches from hours to seconds — ops team could act same-day
Overall SLA% tracked at 57.38% delivery within SLA, giving leadership a clear benchmark to improve
RTO of 598 orders flagged proactively, helping warehouse teams re-initiate pickups faster
Enabled data-driven conversations between logistics managers and courier partners using factual TAT numbers
Replaced manual Excel reporting, saving the team several hours per week


7. 🎓 Key Learnings

Deepened understanding of logistics KPIs — RTO, TAT, SLA, and how they interconnect in a supply chain
Learned to write complex DAX for rolling time-period comparisons (T-7, T-14 logic)
Improved skills in data modeling for operational/transactional data
Understood the importance of stakeholder communication — dashboard iterations were driven by feedback from ops and management
Gained experience in performance optimization of Power BI reports with large order datasets


8. 🔮 Future Enhancements

Automated Alerts — Set up Power BI alerts or Power Automate flows to notify ops teams when SLA% drops below a threshold
Predictive Analytics — Use historical TAT data to predict delivery delays using ML models (Azure ML integration)
Courier Partner Breakdown — Add drill-through by courier/vendor to identify which partners are causing SLA breaches
Real-Time Refresh — Move from scheduled refresh to DirectQuery or streaming dataset for near real-time visibility
Mobile View — Optimize the dashboard layout for Power BI Mobile for field/warehouse managers
Ongoing Monitoring & Support — Establish a monthly review cadence with stakeholders to update KPI targets, add new cities/regions, and maintain data pipeline health
### Screenshots 

Show what the dashboard looks like

Example: ![Dashboard Preview](https://github.com/rishavanalyst07/Logistics-Dashboard/blob/main/Snapshot%20of%20Logistic%20Dashboard.png).
