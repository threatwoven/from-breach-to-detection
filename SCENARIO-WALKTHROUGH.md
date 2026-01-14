# Scenario Walkthrough – Attack to Detection

> This document provides a step-by-step walkthrough of the simulated attack
> used in the "From Breach to Detection – Purple Team Simulation" project.
> The focus is on attacker behavior, detection gaps, and defensive insights,
> rather than tools or exploitation techniques.

## Phase 1: Initial Access
The attacker gains access through compromised user credentials obtained via a phishing campaign.

---

## Phase 2: Internal Reconnaissance
After gaining access, the attacker observes internal network behavior to understand:
- Common communication patterns
- Systems with low visibility
- Implicit trust relationships inside the network

---

## Phase 3: Lateral Movement
The attacker attempts to move laterally by:
- Reusing credentials across internal systems
- Accessing systems that are rarely used
- Leveraging legitimate administrative tools to avoid detection

---

## Phase 4: Privilege Escalation Attempt
The attacker attempts to increase privileges within the environment, including interactions with Active Directory resources.

---

## Phase 5: Detection Gaps
Several gaps contributed to delayed detection:
- Lack of visibility into abnormal authentication patterns
- Insufficient alerting on lateral movement activity
- Delayed detection of privilege escalation attempts

---

## Phase 6: Blue Team Perspective
Security monitoring was primarily focused on perimeter defenses, resulting in limited visibility into internal attacker behavior.

---

## Phase 7: Purple Team Recommendations
- Improve authentication telemetry and anomaly detection
- Enhance logging and monitoring of lateral movement techniques
- Conduct regular Purple Team simulations to align attack paths with detection rules

---

## Outcome
Aligning offensive techniques with defensive detection reduces attacker dwell time and strengthens the overall security posture.

A detailed step-by-step attack walkthrough is available in `SCENARIO-WALKTHROUGH.md`.


