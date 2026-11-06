# PASTA Threat Modeling (Sneaker App)

## Summary
A guided course lab in which I practiced the seven stages of PASTA (Process for Attack Simulation and Threat Analysis) on a fictional sneaker marketplace mobile app. I defined business objectives and technical scope, reviewed a course-provided data flow diagram and sample attack tree, identified threats and vulnerabilities, and recommended security controls.

## My Role
I completed the PASTA worksheet for the scenario: business objectives, technical scope priorities, threat and vulnerability analysis, review of the course diagrams, and recommended controls. The scenario, worksheet, data flow diagram, and sample attack tree were provided by the course.

## Project Overview

This project documents a guided lab from the Google Cybersecurity Certificate (Assets, Threats, and Vulnerabilities). The lab walks through PASTA to identify security requirements before a new shopping app launches. My answers are in the threat model report. The diagrams linked below are course-provided materials I reviewed.

---

## Scenario

I am on the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app so customers can buy and sell shoes. Accounts, messaging, seller ratings, personal information, and payment processing are part of the product goals. My task was to work through PASTA stage by stage and identify security requirements for the app.

---

## Framework

**PASTA** (Process for Attack Simulation and Threat Analysis), applied as seven stages:

| Stage | Focus in this lab |
|---|---|
| I | Define business objectives |
| II | Define the technical scope |
| III | Decompose the application (data flow) |
| IV | Analyze threats |
| V | Analyze vulnerabilities |
| VI | Attack modeling (attack tree) |
| VII | Risk and impact analysis / recommend controls |

Course materials also referenced common vulnerability sources such as OWASP and the CVE list as study aids.

---

## Key Findings

- **Business priorities:** protect personal information and trust, connect buyers and sellers, and process payments securely while meeting legal requirements.
- **Technical priority:** the SQL database is the first scope area to scrutinize because compromise can expose user data and disrupt purchases. APIs and encryption still need review.
- **Threats considered:** SQL injection against insecure queries, and phishing that steals user or employee credentials.
- **Vulnerabilities considered:** unsafe database queries and excessive permissions, plus inadequate email filtering and phishing awareness.
- **Controls recommended:** MFA, parameterized SQL / prepared statements, least privilege, and phishing awareness training.

---

## Recommended Controls

| Control | What it addresses |
|---|---|
| Multi-factor authentication (MFA) | Reduces account takeover after stolen or guessed passwords |
| Prepared statements with parameterized SQL | Blocks classic SQL injection from untrusted input |
| Least privilege for users and app accounts | Limits damage if a query or account is abused |
| Phishing awareness training for employees | Lowers success of credential-theft emails |

---

## Project Documentation

### [PASTA Threat Model Report](pasta-threat-model-report.md)
Completed Stage I through VII responses, including review notes on the course data flow diagram and sample attack tree.

### Course-provided diagrams
- [Data flow diagram](images/course-data-flow-diagram.png) (course material)
- [Sample attack tree](images/course-attack-tree.png) (course material)

---

## Skills Demonstrated

- Applying PASTA stages to an application scenario
- Separating business objectives from technical scope
- Reading a simple data flow diagram and sample attack tree
- Mapping threats to vulnerabilities and recommended controls
- Documenting a qualitative threat model for stakeholders

---

## What I Learned

- Threat modeling works best when business goals come before technical deep dives.
- A data flow diagram shows where untrusted input enters and where sensitive stores sit.
- An attack tree links a valued asset to attack methods and enabling weaknesses.
- Recommended controls should map to the threats and vulnerabilities you named.
- Course samples are starting points. A real app would need a larger tree and more processes than search alone.

---

## Disclaimer

Fictional course exercise from the Google Cybersecurity Professional Certificate (Coursera). The analysis and recommended controls are from my PASTA worksheet, not live testing or implementation. The data flow diagram and attack tree images are course-provided. The write-up is my own.

## Certificate
Google Cybersecurity Certificate - Assets, Threats, and Vulnerabilities
