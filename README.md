# Project #5: Microsoft Entra ID Protection – NESA IA-02

**Focus:** Practical implementation of Microsoft Entra ID Protection with risk-based Conditional Access policies to detect and respond to identity threats.

**NESA Alignment:** Supports **IA-02 (Identification and Authentication)** by enabling risk-aware adaptive authentication, identity verification, and remediation of suspicious sign-ins — key for UAE government/semi-government compliance (e.g., ADNOC, DEWA, Etisalat/e&, G42, Emirates).

**Environment**  
- Tenant: CyberShield086.onmicrosoft.com (Default Directory, Wipiro organization)  
- Microsoft Entra ID P2 trial activated (December 2025)  
- Region: Configured for low-latency access from India

**Key Achievements**  
- Activated Entra ID P2 license in a free trial tenant  
- Created 3 test users and assigned P2 licenses  
- Configured **report-only** risk-based Conditional Access policies  
- Simulated risky sign-ins using Tor Browser (anonymous IP) and VPN (atypical travel)  
- Generated and verified detections in Identity Protection dashboard

**Setup Details**  
- Test users created and licensed with Microsoft Entra ID P2  
- Report-only policies:  
  - **User risk policy**: Low and above → Require password change  
  - **Sign-in risk policy**: Medium and above → Require multifactor authentication  

**Simulation Results**  
- Triggered detections for Test User One on December 27, 2025 (~12:15 PM)  
- Risk state: **At risk** (likely Anonymous IP address and/or Atypical travel)  
- In report-only mode: Sign-ins were allowed but flagged for review/remediation  
- If policies were enabled, they would enforce MFA or password reset

**Screenshots**  
- [Test users with P2 licenses](/screenshots/01-users-licenses1.png)  
- [Conditional Access policies list](/screenshots/conditional-access-policies.png)  
- [User risk policy details](/screenshots/user-risk-policy-details.png)  
- [User risk grant action](/screenshots/user-risk-grant-action.png)  
- [Sign-in risk policy details](/screenshots/sign-in-risk-policy-details.png)  
- [Sign-in risk grant action](/screenshots/sign-in-risk-grant-action.png)  
- [Risky sign-ins list](/screenshots/risky-sign-ins-list.png)  
- [Risky sign-in details](/screenshots/risky-sign-in-details.png)  
- [Risky users overview](/screenshots/risky-user.png)  
- [Additional users licenses views](/screenshots/users-licenses2.png) / [/screenshots/users-licenses3.png](screenshots/users-licenses3.png)

**Loom Demo Video**  
[Coming soon – walkthrough of simulation, detections, and policy explanation]

**Why this project stands out for UAE Cloud Security Engineer roles**  
Shows end-to-end skills in identity threat detection, risk-based access control, and NESA-aligned configuration using Microsoft tools — highly relevant for ADNOC, DEWA, Etisalat, Emirates, G42, and similar employers.
