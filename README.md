# Dhanashree Mahajan | Aspiring GRC Analyst
**Focus:** Fintech Security | NIST CSF 2.0 | Internal Auditing

Welcome to my GRC portfolio. I specialize in bridging the gap between technical security controls and business risk management.

---

## 📂 Projects

###  [Qualitative Risk Assessment: Qckpay Fintech Case Study](./Qckpay-case-study.md)
*Performed a comprehensive risk assessment for a startup, including risk scoring, policy development, and audit testing.*
# GRCProfessional.github.io
# Qualitative Risk Assessment & Policy Development: Qckpay Fintech Case Study

##  Project Objective
To identify, analyze, and treat critical security risks for Qckpay, a high-growth fintech startup, ensuring alignment with the **NIST CSF 2.0** framework and **PCI DSS** requirements.

##  The Scenario
Qckpay handles sensitive financial data and credit card transactions. As a GRC Analyst, I performed a risk assessment to address vulnerabilities in identity management and business continuity.

##  Risk Management Methodology
I utilized a **Qualitative Risk Assessment** approach based on a 5x5 matrix to determine the priority of identified threats.

### Risk Scoring Criteria
* **Likelihood (1-5):** From 'Rare' to 'Almost Certain.'
* **Impact (1-5):** From 'Insignificant' to 'Catastrophic' (considering financial loss and regulatory fines).
* **Calculation:** Inherent Risk = Likelihood × Impact.

### Primary Risk: Data Breach via Credential Theft
| Risk Factor | Score | Justification |
| :--- | :--- | :--- |
| **Inherent Likelihood** | 4 | High frequency of phishing/brute-force attacks in fintech. |
| **Inherent Impact** | 5 | Potential for total loss of customer trust and heavy PCI DSS fines. |
| **Inherent Risk Score** | **20 (Critical)** | Requires immediate mitigation. |

###  Risk Treatment & Residual Risk
To mitigate the risk of credential theft, I implemented **MFA (Multi-Factor Authentication)** and established a **Password Complexity Standard**.

| Risk State | Likelihood | Impact | Risk Score |
| :--- | :---: | :---: | :---: |
| **Inherent (Before)** | 4 | 5 | **20 (Critical)** |
| **Residual (After)** | 1 | 5 | **5 (Low)** |

**Note:** While the Likelihood decreased because the "barrier to entry" is higher, the **Impact** remains a 5 because a breach of this database would still have catastrophic consequences.

##  Governance: Password & Identity Standard
**Policy Owner:** GRC Department  
**Scope:** All employees, contractors, and third-party partners with access to Qckpay systems.

### Control Requirements
1. **Length:** Minimum of 12 characters.
2. **Complexity:** Must include a mix of uppercase, lowercase, numbers, and special symbols.
3. **MFA:** Multi-Factor Authentication is mandatory for all system logins.
4. **Prohibition:** Passwords must not contain easily guessable information (e.g., "Qckpay2026").

##  Compliance & Audit Verification
To ensure the Password Policy was effectively implemented, I conducted a **Test of Effectiveness (ToE)**.

### Audit Procedure
* **Sample Size:** 50 randomly selected employee accounts.
* **Evidence Source:** System-generated "MFA Enrollment" report.
* **Result:** 48/50 users compliant (96%).
* **Status:** **FAIL.** ### 🛠️ Remediation Plan
Although 96% is high, the 4% gap represents a vulnerability.
1. **Root Cause Analysis:** Identified that the two users were new hires who missed the onboarding security briefing.
2. **Corrective Action:** Automated the MFA setup guide to trigger upon account creation.
3. **Re-testing:** Scheduled a follow-up audit in 30 days to ensure 100% compliance.
