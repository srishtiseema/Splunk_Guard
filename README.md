# Splunk_Guard

Splunk-Guard is a hybrid, ML-driven threat detection system for monitoring USB activity and VPN login anomalies. Built using Splunk's free version, the Machine Learning Toolkit (MLTK), and an interactive Streamlit Web Dashboard, it provides affordable threat detection for smaller teams, prototypes, and educational use.

▶️ Watch Demo: YouTube Overview Video

🌐 Try the Live App: Splunk-Guard Web Dashboard

## 🚀 Project Highlights

- Detects abnormal USB write patterns to flag potential data exfiltration  
- Identifies suspicious VPN logins from unusual geographic locations  
- Streamlit Web App for interactive anomaly detection even without Splunk  
- Splunk dashboards and alerts included for real-time enterprise monitoring  
- Leverages free Splunk tools – NO paid plugins required

 ### ⚡ Features

- *USB Anomaly Detection*: Detects unusual spikes in per-device write volumes
- *VPN Login Anomalies*: Flags geo-distance outliers for potential credential misuse
- *Modes*:
  - *Live Mode* — Connects to your Splunk backend via REST API  
  - *CSV Upload* — Analyze your own USB or VPN logs  
  - *Demo Mode* — Uses built-in synthetic data for offline testing
- Interactive charts, anomaly reports, and CSV exports

  #### 📁 Project Structure

