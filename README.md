###Home Cyber Labs — Security Operations, Vulnerability Management, Detection Engineering
**Welcome to my Home Cyber Labs portfolio — a collection of hands-on cybersecurity projects demonstrating real defensive security skills:**
- Log ingestion & SIEM use
- Vulnerability scanning & remediation
- Detection engineering & incident response
- Documentation and evidence of results
- These labs simulate real SOC workflows and are built using Docker, Elastic Stack, Nessus, Wazuh, and Filebeat — all running locally on macOS.
- Recruiters: Each lab folder contains its own README + evidence/screenshots.

## Repository Structure
```
home-cyber-labs/
├── soc-lab/               # Lab 1: NGINX + Filebeat + Elastic Stack
├── vuln-lab/              # Lab 2: Nessus scan + remediation
└── wazuh-ir-lab/          # Lab 3: Brute force detection (Wazuh SIEM)
```
# Lab 1 — Log Collection & Dashboarding (NGINX → Filebeat → Elasticsearch → Kibana)
- Goal: Build a SOC-style log pipeline to collect HTTP access logs and visualize activity.
- Tech Used: NGINX, Docker, Filebeat, Elasticsearch, Kibana (Lens dashboards)
- Result: Live dashboards showing web traffic volume & HTTP status breakdown.
```
Skills Demonstrated:

Built a full SIEM pipeline (log → parse → visualize)
Used Kibana Discover/Lens to visualize trends
Identified abnormal traffic (404 enumeration attempts)

```
# Lab 2 — Vulnerability Assessment & Remediation (Nessus + OWASP Juice Shop)
- Goal: Perform vulnerability scan, fix issues, prove reduction.
- Tech Used: Nessus Essentials, OWASP Juice Shop (Docker)
- Result: Reduced vulnerabilities by adding secure HTTP headers.
```
Skills Demonstrated:

Vulnerability scanning & CVSS interpretation
HTTP header hardening (security fix)
Before/after fix documentation
Evidence includes Nessus HTML reports.

```
# Lab 3 — SSH Brute Force Detection (Wazuh SIEM + Filebeat + Kibana)
- Goal: Generate real attack traffic, detect it, investigate, and visualize spike.
- Tech Used: Wazuh Manager, Wazuh Agent, Filebeat, Elasticsearch, Kibana
- Result: Brute-force SSH attempts detected, logged, and visualized as spike on dashboard.
```
Skills Demonstrated:

Detection engineering (rule triggered: sshd failed authentication)
Incident investigation workflow (log pivoting, filtering attacker IP)
Dashboard creation for brute-force spike

```
