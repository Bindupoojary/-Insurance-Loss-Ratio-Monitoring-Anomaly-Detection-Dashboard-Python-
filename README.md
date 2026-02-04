Insurance Loss Ratio Monitoring and Anomaly Detection

<hr>
This project simulates an end to end analytics workflow for monitoring insurance business performance using key KPIs like Loss Ratio, Claims Trends, and Customer Success Metrics.

The goal is to proactively detect abnormal spikes in loss ratio and support leadership business reviews through automated reporting and visualizations.
<hr>
Objectives

Calculate core insurance KPIs such as Loss Ratio

Track monthly performance trends

Monitor customer success metrics like CSAT, NPS, and First Call Resolution

Detect anomalies in loss ratio using statistical z score monitoring

Export monthly KPI reports and alert summaries
<hr>
Dataset

A synthetic dataset of 30,000 insurance policy records was created with realistic premium and claims patterns.

Included fields:

Policy type

Region

Channel

Premium collected

Claim amount

Loss ratio

CSAT score

NPS score

FCR flag

Ticket resolution time
<hr>
Dataset file:
insurance_loss_ratio_dataset.csv
<hr>
Key Metrics Tracked
Insurance KPI

Loss Ratio = Total Claims Paid / Total Premium Collected

Customer Success KPIs

Average CSAT

Net Promoter Score (NPS)

First Call Resolution Rate (FCR)
<hr>
Project Workflow
1. Data Loading and Cleaning

Load CSV dataset into Pandas

Convert date column into datetime format

Create loss ratio feature
<hr>
2. KPI Reporting

Compute company wide totals for premium and claims

Generate monthly aggregated KPI reports
<hr>
3. Visualization

Monthly loss ratio trend using Matplotlib

Loss ratio breakdown by policy type and region
<hr>
4. Anomaly Detection

Implemented statistical anomaly detection using z score.

Alert condition:

Z score greater than 2 triggers an ALERT month
<hr>
5. Reporting Output

Exports generated:

monthly_kpis_report.csv

loss_ratio_alerts.csv

Example Output

The notebook flags months where claims significantly deviate from normal patterns, helping teams investigate root causes.

Tools Used

Python

Pandas

NumPy

Matplotlib
