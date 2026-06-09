# Threat Detection & Threat Hunting with KQL

A collection of real-world threat hunting investigations developed for Microsoft Defender XDR.

This repository focuses on transforming public threat intelligence reports into actionable, production-ready threat hunts using Kusto Query Language (KQL).

Rather than collecting random queries, each hunt follows a structured methodology designed to emulate a real threat hunting workflow used in modern Security Operations Centers (SOCs).

---

## About

I am a Threat Detection & Response Analyst specializing in:

- Threat Hunting
- Detection Engineering
- Incident Response
- Microsoft Defender XDR
- Microsoft Sentinel
- Threat Intelligence Analysis

This repository serves as my public threat hunting portfolio and documents my approach to transforming threat intelligence into high-fidelity hunting content.

---

## Hunting Methodology

Every hunt in this repository follows the same workflow.

### Step 1 – Threat Analysis

Review the threat report and identify:

- Adversary objectives
- Infrastructure
- Malware families
- Attack techniques
- Potential detection opportunities

### Step 2 – IOC Validation & Enrichment

Extract, validate and enrich:

- Domains
- IP addresses
- Hashes
- Cloud infrastructure
- SaaS services
- Additional reporting sources

The goal is to distinguish high-confidence indicators from noisy or shared infrastructure.

### Step 3 – Initial Hunt Development

Create an initial Microsoft Defender XDR hunt using:

- High-confidence IOCs
- Behavioral indicators
- MITRE ATT&CK techniques

### Step 4 – Hunt Tuning & Validation

Review results and improve signal quality by:

- Removing false positives
- Reducing unnecessary noise
- Improving behavioral specificity
- Validating assumptions

### Step 5 – GitHub Finalization

Publish a production-ready hunt containing:

- Threat summary
- MITRE ATT&CK mapping
- Expected result guidance
- False positive considerations
- Final KQL query

---

## Philosophy

The objective is not to collect KQL queries.

The objective is to transform threat intelligence into high-fidelity hunts through a repeatable methodology focused on:

- Signal quality
- Behavioral analysis
- Threat-informed hunting
- Detection engineering principles
- Production readiness

---

## Featured Hunts

| Hunt | Description | MITRE ATT&CK |
|--------|--------|--------|
| EtherRAT & TukTuk | RAT infrastructure, malware execution and command-and-control activity | T1071, T1105 |
| JOMANGY | Web shell activity and persistence techniques | T1505 |
| BadIIS | IIS malware and malicious module activity | T1505.003 |
| TeslaC2 | Malware-as-a-Service infrastructure and post-exploitation activity | T1071, T1090 |
| EDRChoker | Defense evasion through QoS policy manipulation | T1562.001 |

---

## MITRE ATT&CK Coverage

Current repository coverage includes:

- T1003 – Credential Dumping
- T1055 – Process Injection
- T1071 – Application Layer Protocol
- T1090 – Proxy
- T1105 – Ingress Tool Transfer
- T1486 – Data Encrypted for Impact
- T1505 – Server Software Component
- T1562 – Impair Defenses

Coverage will continue to expand as additional hunts are published.

---

## Repository Structure

Each hunt contains:

- Threat context
- MITRE ATT&CK mapping
- Expected results
- False positive guidance
- Production-ready KQL

---

## Current Focus Areas

- Threat Hunting
- Detection Engineering
- Microsoft Defender XDR
- Threat Intelligence Driven Hunting
- KQL Development

---

## Disclaimer

The content in this repository is intended for educational, research, threat hunting and defensive security purposes.

All threat intelligence is derived from publicly available reporting and is converted into defensive hunting content for Microsoft Defender XDR environments.
