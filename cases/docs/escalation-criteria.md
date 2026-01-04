# Escalation Criteria – SOC Level 1

This document defines the conditions under which an alert or incident should be escalated from SOC Level 1 to SOC Level 2.

The purpose is to ensure consistent decision-making, reduce false escalations, and maintain proper incident handling workflows.

---

## 🔺 When to Escalate to SOC Level 2

An alert should be escalated to SOC Level 2 when one or more of the following conditions are met:

### 1. Confirmed Malicious Activity
- Evidence of data exfiltration
- Confirmed malware execution
- Credential compromise
- Unauthorized access to sensitive systems or data

### 2. Policy Violations Involving Sensitive Data
- External sharing of confidential or regulated information
- DLP alerts involving HR, Finance, or Legal data
- Repeated policy violations by the same user

### 3. Multiple Correlated Indicators
- Multiple alerts linked to the same user, IP, or device
- Patterns suggesting persistence or lateral movement
- Combination of login anomalies and data access events

### 4. High-Risk Users or Assets
- Privileged users (HR, Finance, IT admins)
- Critical systems or sensitive repositories
- External recipients using anonymous or encrypted email providers

### 5. Unclear Intent or Insufficient Context
- Activity cannot be confidently classified as benign
- Lack of visibility prevents proper risk assessment
- Potential impact is high despite limited indicators

---

## 🟢 When NOT to Escalate

An alert may be closed at SOC Level 1 when:

- The activity is confirmed as a false positive
- The behavior aligns with documented business processes
- No additional indicators of compromise are observed
- Risk and impact are assessed as low

---

## 📝 Documentation Requirements Before Escalation

Before escalating, the SOC Level 1 analyst must ensure:

- Alert details and timeline are documented
- Relevant evidence is attached (screenshots, metadata)
- Initial assessment and rationale are clearly written
- Recommended next steps are included

---

## 🎯 Goal of Escalation

Escalation is not an admission of failure.  
It is a controlled handoff to ensure incidents are handled at the appropriate level of expertise and authority.
