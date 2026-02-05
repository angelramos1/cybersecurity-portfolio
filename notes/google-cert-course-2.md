# Google Cybersecurity Certificate - Course 2 Notes
## Security Frameworks and Controls

**Course Completed:** January 2026

---

## Table of Contents
- [Module 1: Security Domains & Risk Management](#module-1)
- [Module 2: Security Frameworks & Controls](#module-2)
- [Module 3: SIEM Tools & Logs](#module-3)
- [Module 4: Incident Response Playbooks](#module-4)

---

## Module 1: Security Domains & Risk Management

### Key Concepts

**Security Posture:** An organization's ability to manage its defense of critical assets and data, and react to change.

### CISSP Security Domains

**1. Security and Risk Management**
- Defines security goals and objectives
- **Risk mitigation:** Process of having procedures and rules to quickly reduce impact of risks like breaches
- **Compliance:** Primary method to develop internal security policies, regulatory requirements, and independent standards
- **Business continuity:** Organization's ability to maintain productivity by establishing risk disaster recovery plans

**2. Asset Security**
- Focuses on securing digital and physical assets
- Handles storage, maintenance, retention, and destruction of data
- Ensures PII/SPII is securely handled and protected (whether stored, transferred, or collected)
- Example: Overseeing hard drive destruction to ensure private data can't be accessed

**3. Security Architecture and Engineering**
- Optimizes data security through effective tools, systems, and processes
- **Shared responsibility:** All individuals take active role in lowering risk and maintaining security

**4. Communication and Network Security**
- Manages and secures physical networks and wireless communications
- Keeps data/communications safe on-site, in cloud, or remote
- Example: Removing insecure bluetooth/public wifi access at organizational level

**5. Identity and Access Management (IAM)**
- Controls access and authorization to keep data secure
- Goal: Reduce overall risk to systems and data
- **Components:**
  - **Identification:** User verifies who they are (username, access card, biometrics)
  - **Authentication:** Verification process (password, PIN)
  - **Authorization:** Level of access based on role
  - **Accountability:** Monitoring and recording user actions

**6. Security Assessment and Testing**
- Conducts security control testing
- Collects and analyzes data
- Conducts security audits to monitor risks, threats, vulnerabilities
- Example: Auditing user permissions to validate correct access levels

**7. Security Operations**
- Conducts investigations and implements preventative measures
- Responds to active attacks with urgency
- Performs digital forensic investigations after incidents
- **Key activities:** Training, documentation, intrusion detection, SIEM tools, incident management, playbooks

**8. Software Development Security**
- Uses secure coding practices
- Integrates security into software development lifecycle
- Security reviews at each phase: design review, code reviews, penetration testing

### Threats, Risks, and Vulnerabilities

**Threat:** Any circumstance or event that can negatively impact assets
- Example: Social engineering attacks, phishing

**Risk:** Anything that can impact confidentiality, integrity, or availability of an asset
- Likelihood of a threat occurring
- **Risk levels:**
  - **Low risk:** Public information (website content, published research)
  - **Medium risk:** Information that may cause some damage (quarterly earnings)
  - **High risk:** Protected by regulations/laws (PII, SPII, intellectual property)

**Vulnerability:** A weakness that can be exploited by a threat
- Examples: Outdated firewall/software, weak passwords, unprotected data, people
- Note: Both vulnerability AND threat must be present for risk to exist

**Key Impacts:**
- **Financial:** Interrupted services, correction costs, fines for non-compliance
- **Identity theft:** PII/SPII sold or leaked through dark web
- **Reputation:** Loss of customers, bad press, legal penalties

### Layers of the Web
- **Surface web:** Publicly accessible content
- **Deep web:** Requires authorization (e.g., organization's intranet)
- **Dark web:** Requires special software, often used by criminals

### NIST Risk Management Framework (RMF)

1. **Prepare:** Monitor risks and identify controls before breach occurs
2. **Categorize:** Develop risk management processes considering CIA impact
3. **Select:** Choose and document controls that protect organization
4. **Implement:** Execute security and privacy plans
5. **Assess:** Determine if controls are implemented correctly
6. **Authorize:** Be accountable for security and privacy risks
7. **Monitor:** Be aware of how systems are operating

### Common Risk Management Strategies
- **Acceptance:** Accept risk to avoid disrupting business
- **Avoidance:** Create plan to avoid risk altogether
- **Transference:** Transfer risk to third party
- **Mitigation:** Lessen impact of known risk

### Common Threats & Vulnerabilities

**Threat Examples:**
- **Insider threats:** Staff/vendors abuse authorized access
- **Advanced Persistent Threats (APTs):** Unauthorized access maintained over extended period

**Risk Factors:**
- External risk
- Internal risk
- Legacy systems
- Multiparty risk
- Software compliance/licensing

**Notable Vulnerabilities:**
- ProxyLogon (Microsoft Exchange)
- ZeroLogon (Netlogon authentication)
- Log4Shell (Java code execution)
- PetitPotam (NTLM theft)
- Security logging/monitoring failures
- Server-side request forgery

---

## Module 2: Security Frameworks & Controls

### Security Frameworks
Guidelines used for building plans to help mitigate risk and threats to data and privacy.

**Key Uses:**
- Create plans that increase employee awareness
- Help organizations adhere to compliance laws (e.g., HIPAA)
- Address both virtual and physical security

### Security Controls
Safeguards designed to reduce specific security risks.

**Three Common Types:**

**1. Encryption**
- Converts data from readable (plaintext) to encoded format (ciphertext)
- Ensures confidentiality of sensitive data
- Ciphertext unreadable until decrypted

**2. Authentication**
- Verifies who someone is
- Basic: Username and password
- Advanced: Multi-factor authentication (MFA) - password + security code/biometrics
- **Biometrics:** Unique physical characteristics (fingerprint, eye scan, palm scan)
- Vulnerable to vishing (voice exploitation to steal identity)

**3. Authorization**
- Grants access to specific resources within system
- Verifies permission to access resource

### Specific Frameworks

**Cyber Threat Framework (CTF)**
- Developed by U.S. government
- Provides common language for describing cyber threat activity
- Helps professionals analyze and share information efficiently

**ISO/IEC 27001**
- Internationally recognized framework
- Manages security of assets (financial info, intellectual property, employee data)
- Outlines requirements for information security management system
- Provides collection of controls (not required to use specific ones)

### Control Categories

**Physical Controls:**
- Gates, fences, locks
- Security guards
- CCTV, surveillance cameras, motion detectors
- Access cards/badges

**Technical Controls:**
- Firewalls
- MFA
- Antivirus software

**Administrative Controls:**
- Separation of duties
- Authorization
- Asset classification

### The CIA Triad

Model that helps organizations consider risk when setting up systems and security policies.

**Confidentiality**
- Only authorized users can access specific assets/data
- "Need to know" basis
- Principle of least privilege limits access to what's needed for job

**Integrity**
- Data is correct, authentic, and reliable
- **Cryptography:** Transforms data so unauthorized parties can't read or tamper
- **Encryption:** Converts data from readable to encoded format
- Difference: Cryptography = transforms data; Encryption = converts to encoded format

**Availability**
- Data accessible to those authorized to use it
- Systems must function properly for timely and reliable access

### NIST Cybersecurity Framework (CSF)

Voluntary framework of standards, guidelines, and best practices to manage cybersecurity risk.

**Six Core Functions:**

**1. Govern**
- Establishes cybersecurity governance structures
- Sets clear objectives and leadership commitment
- Develops comprehensive risk management strategy
- Creates the master plan

**2. Identify**
- Manages cybersecurity risk and its effect on people and assets
- Example: Monitor systems/devices for potential security issues
- Like knowing your house - strengths, weaknesses, what to protect

**3. Protect**
- Strategy to protect through policies, procedures, training, and tools
- Study historical data and improve policies
- Prepares defenses

**4. Detect**
- Identifies potential security incidents
- Improves monitoring capabilities
- Example: Review security tool setup to ensure proper alerting
- System that warns when something's wrong

**5. Respond**
- Proper procedures to contain, neutralize, and analyze incidents
- Implement improvements to security process
- Collect and organize data, document incidents, suggest improvements

**6. Recover**
- Returns affected systems to normal operation
- Restore systems, data, and assets after incidents

**NIST SP 800-53:** Unified framework for protecting federal government information systems

### OWASP Security Principles

**1. Minimize Attack Surface Area**
- Attack surface = all potential vulnerabilities
- Attack vectors = pathways attackers use (phishing, weak passwords)
- Reduce by disabling features, restricting access, complex passwords

**2. Principle of Least Privilege**
- Users have minimum access required for tasks
- Limits damage from security breach

**3. Defense in Depth**
- Multiple security controls addressing risks different ways
- Example: MFA, firewalls, intrusion detection, permissions
- Creates multiple points of defense

**4. Separation of Duties**
- Prevents individuals from carrying out fraudulent activities
- No one should have privileges to misuse system
- Example: Different people sign and prepare paychecks

**5. Keep Security Simple**
- Avoid unnecessarily complicated solutions
- Complex controls harder to manage collaboratively

**6. Fix Security Issues Correctly**
- Identify root cause quickly
- Correct vulnerabilities
- Test to ensure repairs successful
- Example: Strengthen weak wifi passwords

**7. Establish Secure Defaults**
- Optimal security state = default state
- Should take extra work to make application insecure

**8. Fail Securely**
- When control fails, default to most secure option
- Example: Failed firewall closes all connections

**9. Don't Trust Services**
- Don't explicitly trust third-party partners' systems
- Verify before sharing information

**10. Avoid Security by Obscurity**
- Security shouldn't rely on keeping details hidden
- Should rely on password policies, defense in depth, business limits, etc.

---

## Module 3: SIEM Tools & Logs

### Logs

**Log:** Record of events within an organization's systems and networks

**Common Log Sources:**
- **Firewall logs:** Attempted/established connections (incoming/outbound traffic)
- **Network logs:** Computers/devices entering/leaving network, connections between devices
- **Server logs:** Events related to services (websites, emails, file shares), login attempts

### Security Information and Event Management (SIEM)

Application that collects and analyzes log data to monitor critical activities.

**Benefits:**
- Indexes and minimizes manual review
- Increases efficiency and saves time
- Must be configured and customized for each organization
- Requires continuous updates for new threats

**SIEM Dashboards:**
- Quick access to security information
- Charts, graphs, tables
- Display metrics: response time, availability, failure rate
- Customizable for different stakeholders

### Types of SIEM Tools

**Self-Hosted:**
- Organization installs, operates, maintains on own infrastructure
- Managed by IT department
- Ideal for maintaining physical control over confidential data

**Cloud-Hosted:**
- Maintained by SIEM providers
- Accessible through internet
- Ideal for organizations not wanting to maintain own infrastructure

**Hybrid:**
- Leverages cloud benefits while maintaining physical control

**Cloud-Native:**
- Fully maintained by vendor
- Designed specifically for cloud computing (availability, flexibility, scalability)

### Common SIEM Tools

**Splunk**

*Splunk Enterprise (Self-hosted):*
- Retains, analyzes, searches log data
- Provides real-time security information and alerts

*Splunk Cloud (Cloud-hosted):*
- Collects, searches, monitors log data
- For hybrid/cloud-only environments

**Splunk Dashboards:**
1. **Security Posture:** Last 24 hours of notable events, monitor real-time threats
2. **Executive Summary:** Overall health over time, high-level insights for stakeholders
3. **Incident Review:** Identify suspicious patterns, visual timeline of events
4. **Risk Analysis:** Identify risk per object (user, computer, IP), prioritize mitigation

**Chronicle (Google)**

Cloud-native SIEM tool that retains, analyzes, searches log data.

**Can collect/analyze by:**
- Specific asset
- Domain name
- User
- IP address

**Chronicle Dashboards:**
1. **Enterprise Insights:** Recent alerts, suspicious domains (IOCs), confidence scores
2. **Data Ingestion and Health:** Event logs, log sources, success rates
3. **IOC Matches:** Top threats/risks/vulnerabilities, identify trends
4. **Main:** High-level summary of data ingestion, alerting, event activity
5. **Rule Detections:** Incident statistics, triggered alerts by detection rule
6. **User Sign-in Overview:** User access behavior, identify unusual activity

### Open-Source vs Proprietary Tools

**Open-Source:**
- Often free, user-friendly
- Built by public collaboratively (potentially more secure)
- Allows customization
- Examples: Linux, Suricata

**Proprietary:**
- Developed/owned by company
- Users pay fee for usage/training
- Only owners modify source code
- Limited feature modification
- Examples: Splunk, Chronicle

**Common Misconception:** Open-source less effective/safe - FALSE. Many industry standards are open-source.

### Future: SOAR

**Security Orchestration, Automation, and Response (SOAR)**
- Collection of applications, tools, workflows using automation
- Handles common security incidents with less manual intervention
- Frees analysts for complex, uncommon incidents
- Example: Auto-block account after too many wrong password attempts

---

## Module 4: Incident Response Playbooks

### Playbooks

**Playbook:** Manual providing details about operational actions

**Purpose:**
- Ensures consistent actions regardless of who works the case
- Predefined, up-to-date list of steps for responding to incidents
- Accompanied by strategy outlining team member expectations
- Plan dictates how tasks must be completed

**When to Use Playbooks:**
- Open attacks
- Privacy incidents
- Data leaks
- Denial of service attacks
- Service alerts
- Various other incidents

**Maintenance:**
- Must be updated constantly (living documents)
- Update when: failure identified, industry standards change, cybersecurity landscape changes

### Incident Response Playbook Phases

**1. Preparation**
- Document procedures
- Establish staffing plans
- Educate users
- Mitigate likelihood, risk, and impact

**2. Detection and Analysis**
- Detect and analyze events using defined processes/technology
- Determine if breach occurred
- Analyze possible magnitude

**3. Containment**
- Prevent further damage
- Reduce immediate impact
- High priority to prevent ongoing risks
- Example: Isolate infected system

**4. Eradication and Recovery**
- Complete removal of incident's artifacts
- Eliminate malicious code, mitigate vulnerabilities
- Restore to secure state (IT restoration)
- Example: Restore OS and data from clean backup

**5. Post-Incident Activity**
- Document incident
- Inform leadership
- Apply lessons learned
- Determine root cause
- Implement updates/improvements

**6. Coordination**
- Report incidents throughout response process
- Share information based on established standards
- Ensures compliance requirements
- Allows coordinated response and resolution

### Using Playbooks with SIEM/SOAR

**SIEM + Playbook Example (Malware Alert):**
1. **Assess:** Determine if alert is valid, analyze logs
2. **Contain:** Isolate infected system to prevent spread
3. **Eradicate/Recover:** Remove malware, restore OS, restore data from clean backup
4. **Post-Incident:** Create final report, notify authorities (FBI, etc.)

**SOAR + Playbook:**
- SOAR automates repetitive tasks
- Example: SOAR auto-blocks account after failed login attempts
- Analysts then use playbook to resolve issue

---

## Key Takeaways

### Important Reminders
- **People are the biggest threat to security** - training and awareness crucial
- **Communication is key** - will be working with teams constantly
- **Defense in depth** - multiple layers of security controls
- **Playbooks are living documents** - require constant updates
- **SIEM and playbooks work together** - structured, efficient incident response

### Skills to Highlight
- Security auditing and risk assessment
- Understanding compliance frameworks (PCI DSS, GDPR, SOC 2, HIPAA)
- SIEM tool knowledge (Splunk, Chronicle)
- Incident response
- IAM principles
- CIA Triad application
- NIST frameworks (CSF, RMF)

### Resources
- Medium: Good forum for cybersecurity trends
- OWASP: Security principles and best practices
- NIST: Frameworks and standards

---

*These notes are my personal summary and interpretation of Course 2 concepts. For complete information, refer to the official Google Cybersecurity Certificate course materials.*
