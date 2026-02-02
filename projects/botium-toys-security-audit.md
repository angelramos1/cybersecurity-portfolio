# Security Audit: Botium Toys

**Date:** January 2026  
**Context:** Google Cybersecurity Certificate - Course 2  
**Type:** Mock Security Audit & Risk Assessment  
**Framework:** NIST Cybersecurity Framework (CSF)

## Executive Summary

Conducted a comprehensive security audit for Botium Toys, a small U.S. business with a growing online presence. The audit assessed the company's entire security program, including assets, controls, and compliance with industry regulations.

**Overall Risk Score: 8/10 (High)**

The company has critical security gaps that pose significant risk to business operations, customer data, and regulatory compliance.

## My Role & Contribution

**What Was Provided:**
- Botium Toys scenario and company background
- Scope, goals, and risk assessment report (pre-written)
- List of existing assets and current security state
- Control categories and compliance frameworks to evaluate against

**What I Did:**
- Analyzed the provided risk assessment report
- Completed the controls assessment checklist
- Evaluated compliance against PCI DSS, GDPR, and SOC 2 standards
- Identified gaps between current state and required controls
- Prioritized findings by risk level
- Developed recommendations with implementation timelines
- Created this comprehensive audit report

**Skills Demonstrated:**
- Reading and interpreting security documentation
- Applying security frameworks (NIST CSF, PCI DSS, GDPR, SOC 2)
- Critical thinking to identify security gaps
- Risk prioritization
- Technical writing and documentation

## Company Background

Botium Toys is a small U.S.-based toy retailer with:
- Physical storefront and warehouse
- Growing online e-commerce presence
- International customer base (including EU customers)
- Handles payment card data and customer PII/SPII

## Audit Scope

**In Scope:**
- Entire security program at Botium Toys
- All IT assets and infrastructure
- Internal network and systems
- Compliance with U.S. and international regulations

**Assets Assessed:**
- On-premises equipment for business operations
- Employee devices (desktops, laptops, smartphones, peripherals)
- Retail inventory (on-site and online)
- IT systems: accounting, telecom, database, security, e-commerce, inventory
- Internet access and internal network
- Data retention and storage systems
- Legacy systems requiring manual monitoring

## Audit Goals

1. Assess existing assets and their management
2. Evaluate current security controls
3. Determine compliance with regulations (PCI DSS, GDPR, SOC 2)
4. Identify gaps and provide recommendations
5. Improve overall security posture

## Risk Assessment Findings

### Current State Analysis

**Major Vulnerabilities Identified:**

1. **Inadequate Asset Management**
   - IT department lacks complete visibility of all assets
   - No clear asset classification or criticality assessment
   - Uncertain impact of potential asset loss on business continuity

2. **Access Control Issues**
   - All employees have access to internally stored data
   - Unauthorized access to cardholder data and customer PII/SPII possible
   - No implementation of least privilege principle
   - No separation of duties

3. **Data Protection Gaps**
   - No encryption for credit card data (stored, processed, transmitted)
   - Credit card information stored locally in plain text
   - Customer PII/SPII not adequately protected

4. **Missing Critical Controls**
   - No Intrusion Detection System (IDS)
   - No disaster recovery plans
   - No backups of critical data
   - Weak password policies (not meeting minimum complexity)
   - No centralized password management system

5. **Legacy System Risks**
   - No regular maintenance schedule
   - Unclear intervention methods
   - Potential security vulnerabilities

**Existing Controls (Positives):**
- ✅ Firewall with appropriate security rules
- ✅ Antivirus software (monitored regularly)
- ✅ Data integrity controls
- ✅ Physical security (locks, CCTV, fire detection/prevention)
- ✅ GDPR breach notification plan (72-hour requirement)
- ✅ Privacy policies and procedures documented

## Controls Assessment

### Controls Checklist Results

| Control | Status | Priority |
|---------|--------|----------|
| Least Privilege | ❌ No | CRITICAL |
| Disaster Recovery Plans | ❌ No | HIGH |
| Password Policies | ⚠️ Inadequate | HIGH |
| Separation of Duties | ❌ No | HIGH |
| Firewall | ✅ Yes | - |
| Intrusion Detection System (IDS) | ❌ No | CRITICAL |
| Backups | ❌ No | HIGH |
| Antivirus Software | ✅ Yes | - |
| Legacy System Monitoring | ⚠️ Irregular | IMPORTANT |
| Encryption | ❌ No | CRITICAL |
| Password Management System | ❌ No | HIGH |
| Physical Locks | ✅ Yes | - |
| CCTV Surveillance | ✅ Yes | - |
| Fire Detection/Prevention | ✅ Yes | - |

## Compliance Assessment

### PCI DSS (Payment Card Industry Data Security Standard)

| Requirement | Status | Finding |
|-------------|--------|---------|
| Authorized access only | ❌ No | All employees can access cardholder data |
| Secure environment | ❌ No | Credit card data stored without encryption |
| Data encryption | ❌ No | No encryption at any touchpoint |
| Password management | ❌ No | Weak policies, no management system |

**Compliance Status:** ❌ NON-COMPLIANT (Critical Risk)

### GDPR (General Data Protection Regulation)

| Requirement | Status | Finding |
|-------------|--------|---------|
| EU customer data privacy | ⚠️ Partial | Procedures exist but controls lacking |
| 72-hour breach notification | ✅ Yes | Plan established |
| Data classification | ❌ No | Not properly classified or inventoried |
| Privacy policies enforced | ✅ Yes | Documented and maintained |

**Compliance Status:** ⚠️ PARTIALLY COMPLIANT

### SOC 2 (System and Organization Controls)

| Requirement | Status | Finding |
|-------------|--------|---------|
| User access policies | ⚠️ Partial | Policies exist but not enforced (no least privilege) |
| Data confidentiality | ❌ No | PII/SPII not adequately protected |
| Data integrity | ✅ Yes | Controls in place |
| Data availability | ❌ No | While data is available, it's available to ALL employees instead of being limited to only authorized individuals who need access to do their jobs |

**Compliance Status:** ❌ NON-COMPLIANT

## Recommendations

Based on the controls and compliance assessment, Botium Toys has several critical security gaps that need immediate attention. The following recommendations prioritize controls by risk level and compliance requirements.

### CRITICAL PRIORITY – Implement Immediately

**Encryption**  
Botium Toys must encrypt all credit card data to comply with PCI DSS requirements. Without encryption, the company risks data breaches, regulatory fines, and loss of payment processing capabilities.

**Least Privilege**  
Currently, too many users have access to sensitive data. Implementing least privilege ensures only authorized personnel can access credit card information and other critical systems. This is required for PCI DSS, GDPR, and SOC 2 compliance.

**Intrusion Detection System (IDS)**  
An IDS is needed to detect potential security threats and attacks in real-time. Without it, Botium Toys cannot identify when systems are being compromised.

### HIGH PRIORITY – Implement Within 60 Days

**Password Policies and Password Management System**  
Strong password requirements and a centralized password management system will prevent unauthorized access. This is required for PCI DSS compliance.

**Disaster Recovery Plans and Backups**  
Regular backups and disaster recovery procedures ensure business continuity if systems fail or data is lost. This protects against ransomware, hardware failure, and other disasters.

**Separation of Duties**  
No single employee should have complete control over critical processes. This reduces fraud risk and is required for SOC 2 compliance.

### IMPORTANT – Implement Within 90 Days

**Manual Monitoring for Legacy Systems**  
Older systems require dedicated monitoring to identify vulnerabilities and ensure they don't create security gaps.

**GDPR Compliance Procedures**  
Botium Toys must establish procedures to notify EU customers within 72 hours of a data breach, classify customer data properly, and document privacy policies. Non-compliance could result in significant fines.

### Summary

Botium Toys currently fails to meet PCI DSS, GDPR, and SOC 2 compliance requirements. Immediate implementation of encryption, least privilege, and an IDS is critical to protect customer data and avoid regulatory penalties. Additional controls like password management, disaster recovery plans, and separation of duties should follow within 60 days to establish a strong security posture.

## Impact Analysis

**If controls are not implemented:**

- **Financial:** Potential fines from PCI DSS, GDPR violations (€20 million or 4% of revenue)
- **Operational:** Loss of payment processing ability, business disruption
- **Reputational:** Customer trust erosion, negative publicity from data breach
- **Legal:** Lawsuits from affected customers, regulatory investigations

## Key Learnings

Through this audit, I learned:

1. **Risk Assessment Methodology:** How to systematically evaluate an organization's security posture using frameworks like NIST CSF

2. **Compliance Requirements:** Understanding PCI DSS, GDPR, and SOC 2 standards and their practical implications

3. **Prioritization:** How to rank security issues by risk level and business impact

4. **Defense in Depth:** The importance of layered security controls rather than relying on single solutions

5. **Asset Management:** Critical importance of knowing what assets you have before you can protect them

6. **Business Impact:** Security isn't just technical - it directly affects business operations, customer trust, and regulatory standing

## Reflection

This security audit exercise demonstrated how to apply security frameworks to a real-world scenario. While the scope and risk assessment were provided, I had to critically analyze the information, apply my understanding of security controls, and make judgments about compliance.

The most challenging part was prioritizing which controls were most critical - there were many gaps, but I had to think about business impact and regulatory requirements to determine what needed immediate attention versus what could wait 60-90 days.

What struck me most was the compliance risk - without encryption alone, the company violates PCI DSS and could lose the ability to process payments entirely. This shows how security isn't optional; it's essential for business operations.

As a software engineering student, this reinforced that I need to think about security from day one when building applications. Understanding how to evaluate controls and compliance will help me build more secure systems from the start.

The framework-based approach (NIST CSF) was helpful for organizing the assessment systematically. This structured methodology is something I can apply when reviewing security in my own projects or future work.

---

**Tools/Frameworks Used:**
- NIST Cybersecurity Framework (CSF)
- PCI DSS compliance checklist
- GDPR requirements
- SOC 2 criteria
- Risk assessment matrix

**Skills Demonstrated:**
- Security auditing
- Risk assessment
- Compliance evaluation
- Technical documentation
- Business impact analysis
- Prioritization and recommendations
