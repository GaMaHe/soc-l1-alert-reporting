# Case 002 – Email Marked as Phishing After Delivery

## Alert Overview
- Alert Type: Email Marked as Phishing After Delivery
- Severity: Medium
- Status: Awaiting Action
- Detection Source: Email Security System

## Email Details
- Subject: Important Update: Microsoft Teams Pricing Increase
- Sender: Microsoft Support <support@microsoft.com>
- Recipient: Eddie Huffman (IT Manager)
- Body Keywords: 600% price increase; urgent notice; download the report; read the details
- Attached File: REPORT.rar
- Embedded URLs: None

## Security Checks
- SPF: Fail
- DKIM: Fail

## Initial Observation
The email claims to originate from Microsoft Support and creates urgency by referencing a significant pricing increase. The sender address appears spoofed, and both SPF and DKIM checks failed.

The presence of a compressed attachment (RAR) combined with urgency-based language is consistent with phishing or malware delivery attempts.

## Investigation Steps
1. Reviewed email headers and authentication results (SPF/DKIM)
2. Analyzed sender identity and impersonation indicators
3. Evaluated attachment type and delivery method
4. Assessed risk based on recipient role and content context

## Findings
- Sender domain failed email authentication checks
- Email impersonates a trusted vendor (Microsoft)
- Attachment uses a compressed archive format commonly used to evade detection
- No legitimate Microsoft communication pattern observed
- No embedded URLs, but attachment represents a high-risk vector

## Assessment
Based on authentication failures, impersonation indicators, and the presence of a suspicious attachment, the email is highly likely to be malicious.

## Evidence
- Alert details and metadata: evidence/alert-details.png
- Analyst comment and escalation notes: evidence/analyst-comment.png
