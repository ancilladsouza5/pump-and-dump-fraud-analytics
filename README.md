# Social Media-Driven Pump-and-Dump Detection Framework
## Capital Markets Fraud Analytics Portfolio Project

### Project Overview
A data-driven financial crime analytics framework investigating social media-driven market manipulation in the Indian stock market. Using data from SEBI enforcement actions, this project runs an **Event Study Analysis** on an SME scrip (**Afcom Holdings Ltd**) to quantify how coordinated Telegram alerts induce artificial retail liquidity, leading to rapid asset crashes.

* **Compliance Scope:** SEBI PFUTP Regulations & Bharatiya Nyaya Sanhita (BNS) Sec. 318(4)

---

### Key Fraud Metrics

| Investigative Parameter | Analytical Value | Operational Significance |
| :--- | :--- | :--- |
| **Total Illicit Gains Confiscated** | ₹20.25 Crore | Disgorgement value impounded from 7 operators |
| **Manipulated Ecosystem** | 82 Scrips | Multi-account mule network distribution scale |
| **Pre-Promotion Base Volume** | 10,500 Shares/day | Historical baseline liquidity ($T-3$ to $T-1$) |
| **Peak Manipulation Volume** | 310,000 Shares | Induced volume spike at the $T+2$ execution window |
| **Calculated Volume Delta** | **+2,852%** | Statistical anomaly flagging market manipulation |
| **Retail Capital Haircut** | **62.5% Loss** | Peak-to-crash price delta (₹80 to ₹30) |

---

### Event Study Timeline (Afcom Holdings Ltd)
* **T−3 to T−1 (26-Jul to 28-Jul) | Accumulation:** Operators quietly buy shares under deep information asymmetry. Price stable at ₹45; volume at a 10,500 base.
* **T (29-Jul) | Pump Phase:** Coordinated stock tips drop across public Telegram channels. Volume jumps to 180,000; price hits ₹65.
* **T+1 (30-Jul) | Retail FOMO:** Induced retail buying drives price to its peak of **₹80** on a 250,000 volume.
* **T+2 (31-Jul) | Dump Phase:** Admins post *"Today try to sell Afcom"*. Operators execute contrary positions, dumping shares into retail buy queues at peak volume (**310,000 shares**).
* **T+3 (01-Aug) | Crash / Liquidity Vacuum:** Volumes dry up (45,000). Stock hits consecutive lower circuits, crashing to **₹30** and locking retail capital into a **62.5% trap**.

---

### Visual Analytics Preview
![Excel Fraud Analytics Dashboard](dashboard/excel_dashboard_preview.png)

---

### Proactive Surveillance Framework
1. **Alternative Data Sourcing:** Automated web scrapers target Telegram/WhatsApp APIs. **Natural Language Processing (NLP)** flags high-risk financial triggers (*"upper circuit guaranteed"*, *"jackpot share"*).
2. **Cross-Correlative Engine:** Matches text timestamps with live order books. Jumps in volume delta exceeding **$+500\%$ within a 15-minute window** of a social broadcast trigger automated forensic alerts.
3. **SME Sentinel Protocols:** Implements volume-weighted dynamic circuit breakers on low-float stocks to block mass contrary-position dumping into brief artificial liquidity windows.

---

### Repository Structure
* `/data/raw/`: Original SEBI macro metrics and case parameters.
* `/data/processed/`: Contains `sebi_fraud_event_study.xlsx` with cleaned mathematical workflows.
* `/dashboard/`: High-resolution screenshots of the trade lifecycle analytics.
* `/presentation/`: The final investigation slide deck: `pump_and_dump_investigation_deck.pptx`.

**Keywords:** *Fraud Analytics, Market Surveillance, Event Study, SEBI PFUTP, Order Book Anomalies, Asset Disgorgement, Induced Liquidity.*
