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

```plaintext
.vscode/               # Devcontainer settings
├── .devcontainer/
├── .streamlit/
├── Splunk_Guard/
│   ├── dashboards/         # Core Splunk content (dashboards, models)
│   ├── mltk_configs/       # Model guides for Splunk MLTK
│   ├── spl_queries/        # SPL scripts and dashboard JSON exports
│   └── screenshots/        # Saved preview images for judges/users
├── sample_data/            # Example USB and VPN log files
├── app.py                  # Streamlit Web Application for local system use
├── demos_app.py            # Alternate Streamlit demo version for public usage
├── requirements.txt        # Python dependencies
├── README.md               # Project overview (this file)
└── LICENSE                 # MIT License

<h3>🛠 Setup &amp; Usage</h3>

<h4>🚀 Streamlit Web App</h4>
<ol>
  <li>
    <strong>Install dependencies:</strong>
    <pre><code class="language-bash">pip install -r requirements.txt</code></pre>
  </li>
  <li>
    <strong>Update</strong> <code>streamlit/secrets.toml</code> with Splunk credentials (for live mode)
  </li>
  <li>
    <strong>Run the app:</strong>
    <pre><code class="language-bash">streamlit run app.py</code></pre>
  </li>
  <li>
    Or use the public link: <a href="#">Splunk-Guard Web Dashboard</a>
  </li>
</ol>

<hr>

<h4>💾 Splunk Backend (Optional)</h4>
<ol>
  <li>Install <strong>Splunk Enterprise (Free Trial)</strong> and <strong>Machine Learning Toolkit (MLTK)</strong></li>
  <li>Ingest <code>usb_logs.csv</code> and <code>vpn_logs.csv</code> into indexes (e.g., <code>splunk_guard</code>, <code>vpn</code>)</li>
  <li>Use provided SPL scripts for field extraction and anomaly model training</li>
  <li>Import dashboards from <code>splunk_guard/dashboards/</code></li>
  <li>Configure alerts using queries in <code>spl_queries/</code></li>
</ol>




