# Defensive Security Intro

**Date Completed:** January 26, 2026  
**Difficulty:** Easy  
**Room Link:** https://tryhackme.com/room/introductivedefensivesecurity

## Overview
This room introduced me to defensive security (blue teaming) - the practice of protecting organizations from cyber attacks. Unlike offensive security which focuses on finding vulnerabilities, defensive security is about monitoring, detecting, and responding to threats in real-time.

## Key Concepts Learned

### Core Responsibilities of Defensive Security Teams

**1. Monitoring and Detecting**
- Continuously observing network and system activity for suspicious behavior
- Example: Detecting logins from unusual locations (like a London employee logging in from another country)

**2. Incident Response**
- Quickly responding when threats are confirmed
- Process includes: containing the threat, removing it, and restoring normal operations

**3. Threat Intelligence**
- Gathering information about attackers' methods, targets, and trends
- Using this intel to strengthen defenses proactively

**4. Vulnerability Management**
- Identifying and fixing software/system flaws before attackers can exploit them
- Can be done manually or with automated tools

**5. Investigation and Analysis**
- Separating normal activity from suspicious behavior
- Deep analysis to uncover insights about potential threats

### Defensive Security Roles

I learned about different roles in a defensive security team:
- **SOC Analyst** - Frontline monitoring of network/system events
- **Incident Responder** - Investigates and responds to active security incidents
- **Security Engineer** - Develops and maintains security tools and systems
- **Digital Forensics Analyst** - Analyzes evidence after incidents to understand what happened

### Key Defensive Technologies

**Security Operations Centre (SOC)**
- The defensive security command center
- Operates 24/7/365
- Main activities: reviewing alerts, investigating anomalies, responding to incidents

**SIEM Systems (Security Information and Event Management)**
- Central hub for all security data from across the organization
- Acts like a "radar" for the digital environment
- Aggregates information from security devices, workstations, servers, etc.
- Critical for understanding what's happening across the entire IT infrastructure

**Other Defensive Measures:**
- Employee training (especially phishing awareness)
- Intrusion Detection Systems (IDS) - network surveillance
- Firewalls - control what traffic enters the network
- Security policies - ensure correct system usage

## Hands-On Practice

**Scenario:** Protecting FakeBank from an ongoing attack

**Task:** Block a malicious IP address that was attacking the system

**What I Did:**
- Identified the attacking IP address through monitoring
- Used the provided security tools to block the IP
- Successfully prevented the attacker from continuing their assault

**Result:** Successfully defended the FakeBank application by blocking the threat

## Key Takeaways

1. **Defensive security is proactive, not just reactive** - it's about constant monitoring and preparation, not just responding after attacks happen

2. **Defense is a team effort** - multiple specialized roles work together (SOC analysts, incident responders, forensics experts, engineers)

3. **Visibility is crucial** - SIEM systems and centralized monitoring are essential because you can't defend against what you can't see

4. **Human element matters** - employee training is a critical defensive layer since attackers often target people, not just systems

## Reflection

This room showed me the "other side" of cybersecurity. While offensive security (from the previous room) is exciting and technical, defensive security requires constant vigilance and quick decision-making. 

I'm interested in how defensive teams stay alert during long monitoring shifts and how they prioritize which alerts to investigate first when multiple things are happening at once.

As a software engineering student, understanding defensive security helps me think about how to build applications that are easier to monitor and defend - like proper logging, alert mechanisms, and security controls built-in from the start.

## Offensive vs Defensive Security

Having now completed both intro rooms, I can see how they complement each other:
- **Offensive (Red Team):** Finds vulnerabilities by thinking like an attacker
- **Defensive (Blue Team):** Protects systems by detecting and responding to threats

Both perspectives are valuable - knowing how attackers think helps defenders anticipate threats, and understanding defense helps attackers test the most critical areas.
