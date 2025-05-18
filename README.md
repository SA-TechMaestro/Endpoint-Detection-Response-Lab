# 🛡️ Generating and Managing EDR

This project documents a hands-on cybersecurity lab focused on endpoint detection and response (EDR). Using a custom home lab environment, I simulated real-world attack scenarios and used **LimaCharlie** and **Sliver** to monitor activity, create detection rules, and respond to threats.

---

## 🎯 Objectives

- Simulate malicious endpoint activity in a safe lab environment
- Analyze telemetry and event logs using LimaCharlie
- Create and refine detection rules for attacks such as LSASS dumping
- Test alert generation and response mechanisms using Sliver

---

## 🧰 Tools & Technologies

- **LimaCharlie** – Telemetry collection, timeline analysis, rule creation  
- **Sliver (C2 Framework)** – Simulating attacks and command execution  
- **VirusTotal** – Hash lookups and signature checks  
- **Windows & Linux Virtual Machines**  
- Educational resources: [SANS](https://sans.org), [CISA](https://cisa.gov), Microsoft blogs

---

## 🔍 Key Activities

### 📡 Monitoring & Detection
- Analyzed telemetry and event logs using LimaCharlie
- Detected unsigned network connections and privilege changes
- Used VirusTotal to inspect custom file hashes
- Explored LimaCharlie’s Timeline for filtering and correlation

### ⚔️ Detection & Response
- Simulated LSASS dumping using `procdump` via Sliver
- Created custom detection rules based on process access (e.g., `lsass.exe`)
- Validated alert generation using real-time testing
- Blocked volume shadow copy deletion to simulate ransomware defense

---

## 🧠 Lessons Learned

- Gained practical exposure to endpoint monitoring and detection logic
- Learned how to simulate and analyze real attack behavior
- Practiced tuning detection rules to reduce false positives
- Reinforced understanding of attacker behaviors and EDR visibility

---

## 📂 Repo Contents

| File / Folder | Description |
|---------------|-------------|
| `report.md` | Full write-up of the lab process and findings |
| `/images/` | Screenshots of telemetry, rules, detections |
| `/resources/` | Reference links and documentation notes |

---

## ✅ Future Improvements

- Add MITRE ATT&CK mapping to each simulated technique  
- Expand rule coverage to other attack vectors  
- Introduce automation via scripting in future labs
