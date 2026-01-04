# SOC Level 1 Investigation Methodology

This document describes the standard investigation methodology followed for all alerts documented in this repository.

The methodology reflects common SOC Level 1 operational practices and is designed to ensure consistency, accuracy, and proper escalation decisions.

---

## 🎯 Objectives

The primary objectives of the SOC Level 1 investigation process are:

- Quickly identify and triage security alerts
- Distinguish false positives from potential incidents
- Assess risk and potential impact
- Document findings in a clear and auditable manner
- Escalate confirmed or high-risk cases to SOC Level 2 when required

---

## 🔍 Investigation Workflow

Each alert is handled using the following structured workflow:

### 1. Alert Review
- Identify alert type, source, and assigned severity
- Review timestamp, user, asset, and detection context
- Validate that the alert is actionable

### 2. Context Analysis
- Analyze user behavior and historical activity
- Review source and destination details (IP, domain, email, device)
- Identify relevant indicators of compromise (IOCs), if present

### 3. Risk and Impact Assessment
- Assess likelihood of malicious intent
- Evaluate sensitivity of affected data or systems
- Consider user role and asset criticality

### 4. Alert Classification
Based on the available evidence, classify the alert as:
- **False Positive** – Benign activity with no security risk
- **Suspicious Activity** – Unusual behavior with limited indicators
- **Confirmed Incident** – Verified malicious or policy-violating activity

### 5. Documentation
- Record findings and reasoning in the case analysis
- Attach relevant evidence (screenshots, metadata)
- Ensure timelines and observations are clearly documented

### 6. Escalation Decision
- Determine whether escalation criteria are met
- Escalate to SOC Level 2 when required
- Close the alert if no further action is needed

Escalation decisions follow the criteria defined in `docs/escalation-criteria.md`.

---

## 📝 Documentation Standards

All SOC Level 1 investigations must:
- Use clear, factual, and neutral language
- Avoid assumptions or attribution without evidence
- Include timestamps and relevant context
- Support conclusions with documented evidence

---

## 🔄 Continuous Monitoring

Alerts closed at SOC Level 1 may still require:
- Ongoing monitoring for related activity
- Re-evaluation if new indicators appear
- Correlation with future alerts

---

## 📌 Scope and Limitations

This methodology applies to **training-based, simulated SOC environments** and does not imply access to production systems or real organizational data.

The focus is on analytical process, documentation quality, and escalation discipline rather than automated detection or response tooling.
