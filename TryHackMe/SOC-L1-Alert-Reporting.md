# SOC L1 Alert Reporting

## Lab Information

**Platform:** TryHackMe  
**Path:** SOC Level 1  
**Module:** SOC Team Internals  
**Focus:** Alert Reporting, Escalation, and SOC Communication

## Key Concepts Learned

- Alert Reporting
- Alert Escalation
- SOC Communication
- True Positive and False Positive classification
- L1 to L2 escalation workflow
- Writing clear analyst comments
- Using the Five Ws in alert reports

## The Five Ws

A useful SOC alert report should answer:

- **Who** — Which user or account was involved?
- **What** — What activity occurred?
- **When** — When did the activity happen?
- **Where** — Which host, IP, URL, or system was involved?
- **Why** — Why was the alert classified as True Positive or False Positive?

## Alert Reporting Workflow

1. Assign the alert to yourself.
2. Move the alert to **In Progress**.
3. Investigate the available evidence.
4. Determine the appropriate verdict.
5. Write a clear analyst comment.
6. Escalate to L2 when deeper investigation or remediation is required.

## Escalation

Alerts may require escalation when:

- The activity indicates a serious cyberattack.
- Deeper investigation is required.
- Host isolation or password reset may be needed.
- Malware removal or other remediation is required.
- Communication with other teams is necessary.
- The L1 analyst needs assistance from a senior analyst.

## Practical Investigation Experience

During the lab, I investigated a suspicious phishing email that contained an archive attachment and failed email authentication checks.

I documented the evidence using a structured analyst comment, classified the activity, and escalated the alert to an L2 analyst.

I also investigated suspicious Active Directory discovery activity where command execution was associated with a reverse shell process on a Windows server.

The process chain and discovery commands were used to identify the activity as malicious and escalate the alert for further investigation and containment.

## SOC Communication

Effective SOC communication includes:

- Contacting L2 when escalation is required.
- Using alternative communication methods if a user's account may be compromised.
- Informing senior analysts during high-volume or critical alert situations.
- Reporting missed or incorrectly classified malicious activity immediately.
- Reporting SIEM or logging issues instead of ignoring incomplete alerts.

## Skills Practiced

- Alert Investigation
- Alert Reporting
- Analyst Comment Writing
- Alert Escalation
- Phishing Analysis
- Process Chain Analysis
- Active Directory Discovery Analysis
- SOC Communication
- Incident Triage
