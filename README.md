# Network Security - Projects 3 & 4: System Hardening

**Course:** [Insert Course Name/Number Here - e.g., CSEC 4XXX]
**Institution:** [Insert Institution Name Here]
**Group:** Group 2
**Date:** April 29, 2025

**Group Members:**
* Bryan Lim [cite: 34]
* Raquel Lugo [cite: 34]
* Grzegorz Rudnicki [cite: 34]
* Jacob Garcia [cite: 34]
* Casey Sharp [cite: 34]

## Project Overview

This repository contains the deliverables for Project 3 and Project 4, focusing on network topology management, virtual machine hardening, shell scripting, and security evaluation.

**Project 3 Goals:**
* Gain experience managing network topologies.
* Gain experience hardening virtual machines and creating plans of action.
* Gain experience writing and executing shell commands and bash scripts.
* Gain experience evaluating system security and performing cost-benefit analysis.

**Project 4 Goals:**
* Gain experience evaluating the security of a system.
* Gain experience writing reports of actions taken.

The projects involved planning and executing the hardening of a Metasploitable 2 virtual machine within a simulated network environment, including configuring supporting security systems (Firewall and IDS) on separate servers, followed by an after-action report detailing the process, challenges, and evaluation.

## Repository Contents

This repository includes the following components:

1.  **Project 3 - Plan of Action (`Project3Group2.pdf`):**
    * Details the initial plan, including:
        * Selected Operating Systems (IPFire[cite: 44], Debian [cite: 46]) and rationale[cite: 6, 7].
        * User account specifications[cite: 9].
        * Proposed network topology[cite: 11, 12, 54].
        * Requested port forwarding rules[cite: 13, 14].
        * Outline of planned hardening actions for Metasploitable 2, IPFire, and Debian/Suricata servers[cite: 16].
2.  **Project 4 - After-Action Report (`Project4Group2.pdf`):**
    * Provides a comprehensive report formatted for a CTO, detailing:
        * Executive Summary[cite: 38].
        * Final Network Topology Design and rationale[cite: 41, 48, 54].
        * Detailed description of mitigation actions taken[cite: 56].
        * Full listings and analysis of hardening scripts used[cite: 61, 171, 191].
        * Manual configuration steps for IPFire and Debian/Suricata[cite: 243, 248].
        * Difficulties encountered during deployment (e.g., outdated OS issues, MySQL service failure)[cite: 257, 263].
        * Self-evaluation of strategy effectiveness and limitations[cite: 270].
        * Citations (as applicable within the report)[cite: 286].
3.  **Hardening Scripts:**
    * `Hardningscript3_1.sh` (or `.txt`): The primary Bash script used for the initial comprehensive hardening of the Metasploitable 2 server[cite: 61]. (Content available in `Project4Group2.pdf`, Listing 3.1.1 [cite: 63])
    * `updateandport.sh` (or `.txt`): The secondary script used to refine the local Metasploitable 2 firewall rules with a default DROP policy[cite: 60, 164]. (Content available in `Project4Group2.pdf`, Listing 3.1.2 [cite: 171])
    * *(Note: Ensure these script files exist in the repository alongside the PDFs)*

## Technologies Used

* **Target System:** Metasploitable 2 (Ubuntu 8.04 Base) [cite: 47]
* **Firewall:** IPFire [cite: 44]
* **IDS Host:** Debian Linux [cite: 46] with Suricata [cite: 46]
* **Hardening Tools:** Bash Scripting, `iptables`[cite: 58, 166], `fail2ban`[cite: 58], `auditd`[cite: 58], `aide`[cite: 58], `chkrootkit`[cite: 58], standard Linux utilities.
* **Protocols Managed:** SSH, FTP, Telnet, HTTP, HTTPS, MySQL, PostgreSQL[cite: 14].

## How to Review

* Review `Project3Group2.pdf` [cite: 1] for the initial plan.
* Review `Project4Group2.pdf` [cite: 34] for the detailed execution report, analysis, script contents, and self-evaluation.
* Examine the `.sh` or `.txt` script files for the implementation details of the automated hardening steps.
