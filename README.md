🛡️ Threat Hunting & Detection Engineering (KQL)

This repository contains Kusto Query Language (KQL) detections and threat hunting queries developed for Microsoft Defender XDR / Sentinel environments.

It focuses on identifying real-world attack techniques, reducing false positives, and improving detection quality through structured hunting and analysis.

🎯 Objectives
Develop high-confidence detection logic based on IOCs and behavior
Perform threat hunting investigations using real telemetry
Improve signal-to-noise ratio through tuning and validation
Document findings in a clear, analyst-friendly format

🔍 Use Cases Covered (in the future)
Supply chain attacks
Living-off-the-Land (LOLBins) abuse
PowerShell execution monitoring
Command & Control (C2) detection
Vulnerability scanning vs malicious activity differentiation

🧠 Methodology

Each detection follows a structured approach:

Threat Intelligence Integration
Leveraging public/private IOCs (hashes, domains, IPs)
Behavioral Analysis
Identifying suspicious execution patterns (e.g., PowerShell, rundll32)
Contextual Validation
Reviewing process lineage and parent-child relationships
False Positive Reduction
Excluding known benign tools (e.g., vulnerability scanners)

⚠️ Important Notes
Queries may require environment-specific tuning
Some detections include broad behavioral logic for hunting purposes
Always validate results before creating alerts
