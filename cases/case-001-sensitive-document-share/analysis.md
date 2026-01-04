# Case 001 – Sensitive Document Shared Externally

## Alert Overview
- Alert Type: Sensitive Document Share to External
- Severity: Medium
- Verdict: True Positive
- Detection Source: DLP / SIEM Dashboard

## Summary
A sensitive HR document containing employee records was shared externally to a non-corporate email address, violating internal data protection policies.

## Investigation Findings
- User accessed Google Workspace from a trusted corporate device
- Attempted bulk download of HR folder was blocked by DLP
- Sensitive spreadsheet was subsequently shared externally
- External recipient used ProtonMail (non-corporate domain)
- No additional malicious activity observed after the event

## Assessment
The activity represents a confirmed policy violation involving sensitive data exposure. While no further indicators of compromise were observed, the nature of the data requires escalation and compliance involvement.

## Evidence

- Alert details and metadata: `evidence/alert-details.png`
- Analyst comment and escalation notes: `evidence/analyst-comment.png`
