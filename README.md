# brute-force-detection-splunk
Brute-force detection using Splunk on Linux authentication logs from Kaggle. Includes SPL queries, dashboards, and visualizations for SOC-style threat analysis
# Objectives
•	Analyze Linux authentication logs for failed SSH login attempts
	•	Detect potential brute-force attacks using SPL queries
	•	Identify suspicious IP addresses with repeated failures
	•	Visualize attack patterns and frequency over time
  # Tools Used
  •	Splunk (SIEM platform)
	•	Linux authentication logs (Kaggle dataset)
	•	SPL (Search Processing Language)
	•	Data visualization dashboards
# Detection Methodology
The analysis focused on identifying repeated failed login attempts as indicators of brute-force activity.
# Key Detection Query
index=main sourcetype="csv" "failed password"
# Analysis Approach
•	Filtering failed authentication events
	•	Grouping activity by source IP
	•	Identifying repeated login attempts (threshold-based detection)
	•	Visualizing attack patterns over time
# Visualizations
The Splunk dashboards included:
	•	Bar chart: Failed login attempts by source IP
	•	Filtered list: IPs with repeated suspicious activity (≥5 attempts)
	•	Event table: Login attempts with timestamps and status
	•	Line chart: Attack frequency over time
  # Key Insights
  •	Multiple IP addresses made repeated failed login attempts
	•	Some activity showed signs of possible brute-force attacks
	•	Splunk visualizations helped identify suspicious login patterns over time
  # Skills Demonstrated
  •	SIEM log analysis
	•	Threat detection and investigation
	•	Brute-force attack identification
	•	SPL querying and filtering
	•	SOC-style security monitoring
# Dataset Source
•	Kaggle Linux authentication logs dataset
# Note
This project was built as part of a cybersecurity homelab to develop practical SOC analyst skills in log analysis and threat detection.
Sidiq Fapohunda - Aspiring SOC Analyst | Splunk & Threat Detection Enthusiast.
