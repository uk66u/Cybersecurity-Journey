# SOC L1 Alert Triage

## Lab Information
**Topic:** SOC Alert Triage  
**Focus:** Alert Prioritization, Investigation, and Classification

## Key Concepts Learned

- Event vs Alert vs Incident
- Alert Severity and Status
- Alert Prioritization
- Alert Triage
- True Positive vs False Positive
- Analyst Comments
- Evidence-based investigation

## SOC Workflow

Alert → Prioritize → Assign → In Progress → Investigate → Verdict → Comment → Close

## Investigation Cases

### 1. Potential Data Exfiltration
**Severity:** Critical  
**Verdict:** False Positive

A large amount of traffic was detected to Zoom from a meeting room network.

The traffic showed high amounts of both sent and received data, which was consistent with legitimate video conferencing activity.

---

### 2. Double-Extension File Creation
**Severity:** High  
**Verdict:** True Positive

A suspicious file was downloaded:

`cats2025.mp4.exe`

The file used a double extension to appear like a video while actually being an executable.

No evidence confirmed that the file was executed.

---

### 3. GitHub Repository Download
**Severity:** Low  
**Verdict:** False Positive

The activity involved the React repository from a developers network.

The activity was consistent with legitimate software development.

## Key Takeaway

Do not classify an alert based only on severity.

Always investigate the context and available evidence before making a final verdict.
