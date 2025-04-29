# COSC 4470 - Projects 3 & 4: System Hardening

**Course:** COSC 4470 - Applied Network Security
**Institution:** The University of Texas Permian Basin (UTPB) Odessa
**Group:** Group 2
**Date:** April 29, 2025

**Group Members:**
* Bryan Lim
* Raquel Lugo
* Grzegorz Rudnicki
* Jacob Garcia
* Casey Sharp

## Project Overview

This repository contains the deliverables for Project 3 and Project 4 for COSC 4470, focusing on network topology management, virtual machine hardening, shell scripting, and security evaluation.

**Project 3 Goals:**
* Gain experience managing network topologies.
* Gain experience hardening virtual machines and creating plans of action.
* Gain experience writing and executing shell commands and bash scripts.
* Gain experience evaluating system security and performing cost-benefit analysis.

**Project 4 Goals:**
* Gain experience evaluating the security of a system.
* Gain experience writing reports of actions taken.

The projects involved planning and executing the hardening of a Metasploitable 2 virtual machine within a simulated network environment. This included configuring supporting security systems (a Firewall using IPFire and an IDS using Debian/Suricata) on separate servers. Project 4 provides an after-action report detailing the process, scripts developed, challenges encountered, and a self-evaluation of the hardening effectiveness.

## Repository Contents

This repository includes the following components:

1.  **Project 3 - Plan of Action (`Project3Group2.pdf`):**
    * Details the initial plan submitted for the project, including:
        * Selected Operating Systems (IPFire, Debian) and justifications.
        * User account specifications for each server.
        * The proposed logical network topology.
        * Requested port forwarding rules for external access.
        * An outline of the planned hardening steps for the Metasploitable 2, IPFire, and Debian/Suricata servers.
2.  **Project 4 - After-Action Report (`Project4Group2.pdf`):**
    * Provides a comprehensive report formatted as an explanation to a CTO, detailing:
        * An Executive Summary of the hardening project.
        * The final Network Topology Design implemented and its rationale.
        * Detailed descriptions of the mitigation actions taken on each server.
        * Full listings and analysis of the Bash hardening scripts developed and used on Metasploitable 2.
        * Descriptions of the manual configuration steps performed on the IPFire firewall and Debian/Suricata IDS.
        * A summary of difficulties encountered during deployment (e.g., issues related to the outdated OS, MySQL service failures).
        * A self-evaluation discussing the effectiveness of the chosen strategies and identifying limitations or areas for improvement.
        * References to resources used (as noted within the report/scripts).
3.  **Hardening Scripts:**
    * `Hardningscript3_1.sh` (or `.txt`): The primary Bash script designed for the initial, broad hardening of the Metasploitable 2 server. *(Content included within `Project4Group2.pdf`)*
    * `updateandport.sh` (or `.txt`): The secondary script focused on refining the local Metasploitable 2 firewall (`iptables`) rules, implementing a default DROP policy for enhanced security. *(Content included within `Project4Group2.pdf`)*
    * *(Note: These script files should ideally be present in the repository as separate `.sh` or `.txt` files for direct review, in addition to being documented in the PDF report.)*

## Technologies Used

* **Target System:** Metasploitable 2 (Based on Ubuntu 8.04 LTS "Hardy Heron")
* **Firewall:** IPFire distribution
* **IDS Host:** Debian Linux (minimal install) with Suricata IDS engine
* **Hardening Tools:** Bash Scripting, `iptables`, `fail2ban`, `auditd`, `aide`, `chkrootkit`, `ufw`, standard Linux system administration utilities (`useradd`, `chpasswd`, `sed`, `grep`, etc.)
* **Protocols Managed/Secured:** SSH, FTP, Telnet, HTTP, HTTPS, MySQL (attempted), PostgreSQL.

## How to Review

* Start with `Project3Group2.pdf` to understand the initial project plan.
* Read `Project4Group2.pdf` for the comprehensive after-action report, which includes the execution details, script listings, analysis of outcomes, challenges faced, and the team's self-assessment.
* Examine the individual script files (`Hardningscript3_1.sh`, `updateandport.sh`) if included separately in the repository for the direct implementation code.
