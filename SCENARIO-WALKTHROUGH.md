# Scenario Walkthrough – Attack to Detection

> This document provides a step-by-step walkthrough of the simulated attack
> used in the "From Breach to Detection – Purple Team Simulation" project.
> The focus is on attacker behavior, detection gaps, and defensive insights,
> rather than tools or exploitation techniques.

The attacker gains access through compromised user credentials obtained via a phishing campaign, resulting in legitimate-looking authentication activity.


Phase 2: Internal Reconnaissance

After gaining access, the attacker passively observes internal network behavior to identify:

Common communication patterns

Systems with low visibility and minimal monitoring

Implicit trust relationships within the internal network

This phase focuses on understanding which assets can be accessed without triggering alerts.


Phase 3: Lateral Movement

The attacker attempts to move laterally by:

Reusing valid credentials across internal systems

Accessing rarely used or low-traffic systems

Leveraging legitimate administrative tools to blend in with normal activity

These actions exploit the assumption that internal traffic is inherently trusted.


Phase 4: Privilege Escalation Attempt

The attacker attempts to increase privileges within the environment, including interactions with Active Directory resources, aiming to expand access to higher-value assets.


Phase 5: Detection Gaps

Several detection gaps contributed to delayed response:

Lack of visibility into abnormal authentication patterns

Insufficient alerting for lateral movement behavior

Delayed detection of privilege escalation attempts


Phase 6: Blue Team Perspective

Security monitoring was primarily focused on perimeter-based threats, resulting in limited visibility into post-compromise internal attacker behavior.


Phase 7: Purple Team Recommendations

To reduce attacker dwell time and improve detection maturity:

Improve authentication telemetry and behavioral anomaly detection

Enhance logging and monitoring of lateral movement techniques

Conduct regular Purple Team simulations to align attack paths with detection rules


Outcome

Aligning offensive techniques with defensive detection capabilities reduces attacker dwell time and strengthens the overall security posture.

A detailed step-by-step attack walkthrough is available in `SCENARIO-WALKTHROUGH.md`.


