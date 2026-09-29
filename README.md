# Awesome-Breach-n-Attack-Simulation

# Top Breach & Attack Simulation (BAS) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Adversary Emulation, Continuous Security Validation & Control Testing*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Breach and Attack Simulation (BAS)**. These tools simulate real-world cyberattacks against an organization's infrastructure to validate security controls, test detection capabilities, and measure defensive posture against known threat actor behaviors.

**Examples** include SafeBreach, AttackIQ, Cymulate, Picus Security, XM Cyber, Pentera, Mandiant Security Validation, Scythe, ThreatGen, Verodin, NodeZero, and Horizon3.ai (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom adversary emulation, and transparent security validation — ideal for purple teams, detection engineers, and security researchers building vendor-independent attack simulation programs. A 2024 IEEE study comparing nine open-source adversary emulation tools ranked MITRE Caldera, Metasploit, and Atomic Red Team as the top performers.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[SafeBreach](https://www.safebreach.com/)**  
  Continuous security validation platform with 20,000+ attack methods simulating known threat actor behaviors across the kill chain.

- **[AttackIQ](https://www.attackiq.com/)**  
  Breach and attack simulation platform built on MITRE ATT&CK, enabling continuous validation of security controls with automated attack scenarios.

- **[Cymulate](https://cymulate.com/)**  
  Extended security posture management platform with BAS, automated red teaming, and attack surface validation across email, web, and endpoint vectors.

- **[Picus Security](https://www.picussecurity.com/)**  
  Security validation platform combining BAS with threat intelligence, measuring detection and prevention effectiveness across security stack.

- **[XM Cyber](https://www.xmcyber.com/)**  
  Hybrid cloud exposure management platform simulating attack paths to critical assets, identifying and prioritizing remediation.

- **[Pentera](https://www.pentera.io/)**  
  Automated penetration testing platform simulating full attack chains from external and internal perspectives with actionable remediation.

- **[Mandiant Security Validation](https://www.mandiant.com/)**  
  Advanced attack simulations backed by real-world threat intelligence.

- **[Scythe](https://scythe.io/)**  
  Adversary emulation platform with threat intelligence-driven attack scenarios, purple team collaboration, and detection validation.

- **[ThreatGen](https://www.threatgen.com/)**  
  Cyber range and attack simulation platform with gamified red team/blue team exercises for training and validation.

- **[Verodin](https://www.mandiant.com/)**  
  Security instrumentation platform (now part of Mandiant) validating security controls through automated attack simulations.

- **[NodeZero](https://www.horizon3.ai/)**  
  Horizon3.ai's autonomous penetration testing platform discovering exploitable vulnerabilities and validating attack paths with proof-of-exploit.

- **[Horizon3.ai](https://horizon3.ai/)**  
  Autonomous penetration testing platform (NodeZero) discovering exploitable vulnerabilities and validating attack paths with proof-of-exploit.

## Open-Source GitHub Projects

- **[MITRE Caldera](https://github.com/mitre/caldera)**  
  The leading open-source automated adversary emulation platform, originally developed by MITRE in 2017 and now under Apache Software Foundation incubation. Ranked #1 in a structured IEEE comparison of nine open-source adversary emulation tools. Uses lightweight agents (Sandcat for Windows/macOS/Linux) paired with a central C2 server that schedules and orchestrates ATT&CK-mapped techniques as "abilities" grouped into "adversaries" (playbooks). Supports red team operations, purple team exercises, detection engineering, and continuous security validation. Includes over 1,700 actions covering all post-compromise tactics. Features a built-in learning module with interactive tasks and certification.

- **[Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)**  
  Library of small, focused tests mapped to MITRE ATT&CK techniques, created by Red Canary. Ranked #3 in the IEEE comparison. Each atomic is a unit test for a detection rule — not a campaign platform. The community has created 1,673 atomics covering 49% of all ATT&CK techniques. Executed via PowerShell module Invoke-AtomicRedTeam or manual command execution. Best used as a library of test cases for detection engineering rather than standalone automated emulation.

- **[Infection Monkey](https://github.com/guardicore/monkey)**  
  Open-source, agent-based adversary emulation tool from Guardicore (now Akamai). Designed for testing network propagation and lateral movement with self-propagating agents. Uses a central web server ("Monkey Island") and agents ("Monkeys") that scan and auto-propagate using exploits, fingerprinting for HTTP/MSSQL/SMB/SSH, and configurable credential lists. Can simulate ransomware by encrypting files in specified folders. Not integrated with MITRE ATT&CK framework. Requires more internal expertise to run effectively than Caldera.

- **[OpenBAS](https://github.com/OpenBAS-Platform/openbas)**  
  Open-source breach and attack simulation platform from Filigran (creators of OpenCTI), ISO 22398 compliant. Unique capability to simulate every aspect of an incident — not just technical attacks, but also contextual events like crisis communication, legal aspects, and business impact. Features AI-powered scenario generation, integration with OpenCTI for threat intelligence-driven simulations, and over 1,600 ready-made "injects". Over 4,000 members in Slack community. Shipped as Docker images for easy self-hosting.

- **[Splunk Attack Range](https://github.com/splunk/attack_range)**  
  Open-source project for spinning up instrumented cloud environments to simulate adversary behavior and test detections. Deploys Splunk instances, Windows/Linux servers, optional Kali, Zeek, and Active Directory-style layouts using Terraform and Ansible. Integrates with Atomic Red Team for attack simulation, with telemetry forwarded to Splunk for detection development. 2,082 stars on GitHub.

- **[PurpleSharp](https://github.com/mvelazc0/PurpleSharp)**  
  Adversary simulation tool for Windows Active Directory environments, automating attack simulation against AD remotely. Closest to a functioning agentless adversarial emulation tool for AD, though development has not continued in recent years. Limited scope to Windows AD only, requires administrative credentials and SMB/RPC connectivity.

- **[Stratus Red Team](https://github.com/DataDog/stratus-red-team)**  
  "Atomic Red Team for the cloud" from Datadog — granular attack techniques for AWS, Azure, GCP, and Kubernetes. Does not resolve the shortcomings of Atomic Red Team regarding full attack chain emulation.

- **[Red Team Automation (RTA)](https://github.com/endgameinc/RTA)**  
  Collection of scripts mapped to MITRE ATT&CK TTPs from Endgame. Less comprehensive than Atomic Red Team.

- **[Network Flight Simulator](https://github.com/alphasoc/flightsim)**  
  Utility to generate malicious network traffic and evaluate security controls. Simulates DNS tunneling, ICMP tunneling, DGA traffic, cryptomining traffic, C2 requests, and data exfiltration over SFTP/SSH. 11 modules with differentiated attacks. Command-line only, not classified by MITRE ATT&CK.

- **[APTSimulator](https://github.com/NextronSystems/APTSimulator)**  
  Windows script that uses tools and output files to make a system appear compromised. No GUI, database, or agents — download and run as administrator. Does not simulate malware or classify attacks by MITRE ATT&CK. Not recommended for production environments.

### Additional Strong Open-Source Options

- **VECTR** — Open-source purple team tracking and reporting tool for measuring detection coverage across exercises.
- **DeTT&CT** — Tool for mapping detection coverage against ATT&CK and identifying gaps, complementing attack simulation platforms.
- **CyberBattleSim** — Microsoft's platform for training and testing automated agents based on reinforcement learning in simulated network environments.
- **Bounty Hunter** — Plugin for Caldera that enhances pre-compromise tactics including Reconnaissance, Resource Development, and Initial Access.
- **Metasploit** — Ranked #2 in IEEE open-source adversary emulation comparison, though primarily a penetration testing framework rather than BAS platform.

**Frameworks for building custom BAS programs**: Combine **MITRE Caldera** as the core adversary emulation engine with agent-based execution and ATT&CK-native playbooks. Integrate **Atomic Red Team** as a library of granular tests for detection validation. Use **OpenBAS** for crisis simulation and non-technical incident aspects, especially when integrated with OpenCTI for threat intelligence-driven scenarios. Deploy **Splunk Attack Range** for cloud-based detection engineering labs with full telemetry pipelines. For network-level validation, **Network Flight Simulator** provides malicious traffic generation without endpoint agents.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Attack simulation tools must be used only in authorized environments with proper legal approval. Unauthorized use may violate computer fraud laws.
- Self-hosted open-source solutions require proper infrastructure, security hardening, and ongoing maintenance. BAS tests are not a substitute for penetration testing; they validate known TTPs and cannot discover unknown attack paths.
- The open-source ecosystem provides strong adversary emulation frameworks and detection validation libraries, but full BAS platforms with automated remediation guidance and executive reporting remain primarily commercial offerings.

---

**Made for purple teams, detection engineers, red teamers, and security researchers.**  
Let's make breach and attack simulation more open, transparent, and vendor-neutral.
