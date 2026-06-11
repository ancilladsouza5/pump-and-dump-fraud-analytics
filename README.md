# Social Media-Driven Pump-and-Dump Detection Framework
## Capital Markets Fraud Analytics Portfolio Project

### Project Overview
This repository contains a financial crime analytics framework investigating social media-driven market manipulation in the Indian capital markets. Utilizing data extracted from SEBI enforcement actions, this project performs an **Event Study Analysis** to quantify how coordinated stock recommendations across encrypted messaging platforms (primarily Telegram) induce artificial retail liquidity, resulting in massive wealth destruction.

* **Target Entity Focus:** Afcom Holdings Ltd (SME Scrip Case Study)
* **Primary Compliance Focus:** SEBI Prohibition of Fraudulent and Unfair Trade Practices (PFUTP) Regulations & Bharatiya Nyaya Sanhita (BNS) Sec. 318(4)

---

### Investigative Metrics Summary
An analysis of the core data sheets yields the following verified fraud metrics:

| Analytical Parameter | Value | Investigative Significance |
| :--- | :--- | :--- |
| **Total Illicit Gains Confiscated** | ₹20.25 Crore | Total disgorgement value impounded from the operator network |
| **Manipulated Ecosystem** | 82 Scrips / 7 Operators | Multi-account "Mule Network" distribution architecture |
| **Pre-Promotion Average Volume** | 10,500 Shares/day | Historical baseline volume ($T-3$ to $T-1$) |
| **Peak Manipulation Volume** | 310,000 Shares | Induced volume spike at the $T+2$ execution window |
| **Calculated Volume Delta** | **+2,852%** | Statistical anomaly flagging severe market manipulation |
| **Retail Capital Haircut** | **62.5% Loss** | Peak-to-crash price delta (₹80 to ₹30) creating a liquidity trap |

---

### Event Study Timeline (Afcom Holdings Ltd)
The quantitative lifecycle tracks the exact correlation between social media coordination and market anomalies across a 7-day impact window ($T-3$ to $T+3$):

* **T−3 to T−1 (26-Jul to 28-Jul):** **Accumulation Phase** — Historical baseline trading (10,500 shares/day average) while operators quietly build core long positions under deep information asymmetry. Stock price stable at ₹45.
* **T (29-Jul):** **Pump Phase** — Coordinated alerts broadcast across massive Telegram public channels (accounting for 70% of distribution channel share). Volume surges to 180,000 shares; price jumps to ₹65.
* **T+1 (30-Jul):** **Retail FOMO Phase** — Induced retail buying drives the price to its absolute peak of **₹80** on a massive 250,000 share volume.
* **T+2 (31-Jul):** **Dump Phase** — Telegram admins drop the explicit *"Today try to sell Afcom"* exit message. Operators execute contrary positions, dumping their shares into the retail buy queues, hitting a peak volume of **310,000 shares**.
* **T+3 (01-Aug):** **Crash / Liquidity Vacuum** — Volume instantly vanishes down to 45,000 shares. The stock gets trapped in consecutive lower circuits, crashing to **₹30** and locking retail investors into a **62.5% loss**.

---

### Visual Analytics Preview
Below is the data visualization tracking the inverse correlation between vanishing market liquidity and falling asset prices during the crash phase:

![Excel Fraud Analytics Dashboard](dashboard/excel_dashboard_preview.png)

---

### Proactive Surveillance & Sourcing Framework (The Analyst Solution)
To mitigate these systemic threats before massive capital erosion occurs, this project maps out an enterprise-grade automated detection engine:

1. **Alternative Data Sourcing (External Engine):** Deploying specialized web scrapers across public Telegram APIs, WhatsApp business lists, and X (Twitter) feeds. Using **Natural Language Processing (NLP)**, the engine flags high-risk financial sentiment triggers (e.g., *"upper circuit guaranteed"*, *"target price reached"*, *"jackpot scrip"*).
2. **Cross-Correlative Surveillance (Internal Engine):** Syncing the scraped text timestamps with real-time exchange order books. If an illiquid SME scrip experiences an order book volume variance exceeding **$+500\%$ within a 15-minute window** of a flagged social media broadcast, it automatically triggers an investigative alert.
3. **SME Scrip Sentinel Protocols:** Recommending dynamic, volume-weighted algorithmic circuit breakers specifically tailored to low-float stocks to prevent operators from dumping massive blocks into retail buy orders during brief periods of artificial liquidity.

---

### Repository Structure
* `/data/raw/`: Original SEBI macro metrics and case parameters.
* `/data/processed/`: Contains `sebi_fraud_event_study.xlsx` with cleaned mathematical steps and volume multipliers.
* `/dashboard/`: Hosts high-resolution screenshots capturing the trade lifecycle analysis.
* `/presentation/`: The final investigation slide deck: `pump_and_dump_investigation_deck.pptx`.

**Keywords:** *Fraud Analytics, Market Surveillance, Event Study, SEBI PFUTP, Order Book Anomalies, Asset Disgorgement, Induced Liquidity.*
