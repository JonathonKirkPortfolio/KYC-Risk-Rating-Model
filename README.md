# 🔬 Dual-Use Goods & Chemical Precursor KYC Risk Model

## 📌 Project Overview
This repository contains a functioning, automated Customer Due Diligence (CDD) risk-scoring engine built in Excel. Unlike standard retail banking risk models, this tool is specifically designed for commercial banking compliance departments reviewing corporate clients in the pharmaceutical, chemical logistics, and laboratory supply sectors.

The model targets the critical intersection of financial crime and illicit material diversion, specifically addressing Trade-Based Money Laundering (TBML) and Proliferation Financing vulnerabilities.

## ⚙️ Methodology & Technical Architecture
This tool was built using a strict separation of front-end User Interface and back-end logic to ensure data integrity and prevent accidental manual overrides.

*   **Automated Risk Ingestion:** Utilizes `VLOOKUP` matrices to dynamically score clients based on geography, entity type, and product profiles, pulling from a hidden, protected database.
*   **Strict Data Validation:** Prevents manual entry errors by forcing analysts to select pre-approved regulatory categories via dynamic drop-down lists.
*   **Regulatory Override Logic:** Employs nested `IF(OR(...))` logic to automatically trigger a "HIGH RISK" escalation if a client handles high-risk UN-scheduled chemical precursors or if a Politically Exposed Person (PEP) is identified.
*   **Conditional UI Alerting:** Uses automated conditional formatting to immediately highlight high-risk files requiring Enhanced Due Diligence (EDD) without requiring the analyst to manually calculate the risk tier.

## ⚖️ Regulatory Context (UK Framework)
The risk weights applied in the data matrix are informed by:
1.  **The Joint Money Laundering Steering Group (JMLSG)** guidance regarding trade-based money laundering and high-risk jurisdictions.
2.  **UK Home Office / UNODC classifications** of scheduled precursor chemicals vulnerable to illicit diversion.

## 👤 About the Author
I am an ICA Certified KYC & CDD professional transitioning into financial crime compliance. With nearly five years of experience in high-security forensic laboratory operations, my background is rooted in strict procedural adherence, secure supply chain logistics, and rigorous evidence handling. 

This project demonstrates my ability to translate complex regulatory requirements and forensic-level stock tracking principles into functional, automated compliance controls.

## 📁 How to View the Project
1. Download the `Chemical_KYC_Risk_Model.xlsx` file from this repository.
2. Open the file in Microsoft Excel.
3. On the `Dashboard` tab, use the drop-down menus in Column B to test how altering client variables dynamically changes the overall regulatory risk classification.
