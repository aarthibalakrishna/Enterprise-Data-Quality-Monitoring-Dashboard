# Enterprise-Data-Quality-Monitoring-Dashboard
DMAIC Case Study<br>
Framework: DMAIC Case Study
Tools: Power BI, DAX, SQL, Python (for data profiling)

<h1>Define</h1>
The goal was to establish a centralized monitoring system to improve the Overall DQ Score (currently 65.44%) and ensure all Business Units (BUs) meet a 90% SLA compliance target. 
Key stakeholders include Finance, HR, Operations, Sales, and Supply Chain.

<h1>Measure</h1>
Established baseline metrics using real-time data as of September 30, 2025:
Total Issues Identified: 114.
Average Resolution Time: 4.76 days.
SLA Compliance: Currently at 79.8%, 
falling short of the 90% target.
High-Risk Volume: Identified 18 open issues with a "High" risk rating.

<h1>Analyze</h1>
Using the Issue Pattern Analysis and Root Cause Explorer, I identified the primary drivers of data defects:
Worst Performing BU: Supply Chain leads with 32 total issues.
Top Defect Types: "Out of Range" (specifically in Finance and HR) and "Late Refresh" (prominent in Supply Chain).
System Vulnerability: Issues are tracked across multiple sources, including SAP, Salesforce, WMS, and Oracle.
Critical Fields: The top failing fields impacting downstream reporting are Invoice Date, Amount, and Email.

<h1>Improve</h1>
The dashboard enables targeted interventions by:
Team Accountability: Visualizing issues by owner teams (e.g., DataOps has 114 issues, FinanceOps has 101) to reallocate resources.
Geographic Filtering: Ability to drill down into specific regions like Germany, India, Singapore, UK, and USA to identify localized process failures.
Trend Monitoring: Tracking the DQ Score Trend to ensure that improvements in one BU (like the peak in Finance) are replicated across others.

<h1>Control</h1>
To sustain improvements, the Control and Governance Monitoring page  
tracks:SLA Breach Trends: Monthly tracking to ensure a downward trend in breaches.
Executive Scorecard: A high-level view for leadership to monitor BUs, Systems, and Countries currently below SLA.
Actionable Logs: A detailed "Issue ID" tracker (e.g., ISS-1001, ISS-1004) to monitor real-time status from "Open" to "In Progress".

<h1>Key Technical Features Demonstrated</h1>
Dynamic Visuals: Line charts for monthly trends and horizontal bar charts for BU comparisons.
Complex Filtering: Multi-select slicers for Countries and Business Units.
Conditional Formatting: Red/Yellow/Green indicators for SLA targets (Target: 90% | Red <75%).
Data Modeling: Integrating disparate sources like LegacyApp and Oracle into a unified star schema.
<br>
  <h2>1</h2>
<img width="1291" height="728" alt="image" src="https://github.com/user-attachments/assets/f3d3e724-a45c-4941-bab2-5c7596d34052" />
  <h2>2</h2>
<img width="1300" height="735" alt="image" src="https://github.com/user-attachments/assets/7e6d2679-ec33-4fba-893f-dd807e7cd495" />
  <h2>3</h2>
<img width="1291" height="731" alt="image" src="https://github.com/user-attachments/assets/c475734a-90cc-49fe-82ba-e53895af7a61" />
  <h2>4</h2>
<img width="1296" height="727" alt="image" src="https://github.com/user-attachments/assets/bb5323bd-208e-467a-a32d-89c2978b0235" />


