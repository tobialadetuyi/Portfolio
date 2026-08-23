# security.portfolio / case-studies

**Real findings. Proven impact.**

Penetration testing, vulnerability assessment, and security training case studies — redacted for confidentiality. Every engagement shown here was delivered under formal authorization with measurable impact on client security posture.

---

## About This Portfolio

This repository contains detailed technical case studies from real-world security engagements conducted across multiple domains:

- **Web Applications** — Full-spectrum VAPT, authentication bypass, injection flaws, access control breaches
- **Mobile Security** — Android & iOS penetration testing, runtime instrumentation, API interception
- **Infrastructure & Active Directory** — Domain compromise, Kerberos attacks, lateral movement, privilege escalation
- **Security Training** — ISO 27001:2022 competence-based audit programmes

All engagements were conducted under formal written authorization. Client identities and sensitive operational details are redacted under NDA.

---

## Case Studies

### 1. **Full-Spectrum VAPT — Nigerian Commercial Bank**
- **Scope:** 4 attack surfaces (web app, API, network, Active Directory)
- **Key Findings:** Subdomain takeover (CVSS 9.3), SQL injection, unauthenticated API endpoints, AS-REP roasting
- **Total Findings:** 31 vulnerabilities (3 Critical, 8 High, 12 Medium, 6 Low, 2 Info)
- **Impact:** Unauthorized fund transfers, mass credential theft, regulatory breach potential
- **Reference:** `bank-vapt-full-assessment.html`

### 2. **Full Domain Compromise via Zerologon — Investment Firm VAPT**
- **Scope:** 7 targets (Domain Controller, web apps, cloud, ERP, SharePoint)
- **Critical Finding:** CVE-2020-1472 (Zerologon) — Domain Controller fully compromised
- **Attack Chain:** Reconnaissance → DC machine account reset → NTLM hash dump → Pass-the-hash → SYSTEM shell
- **Key Exploits:** Zerologon, NTLM relay (LLMNR/NBT-NS poisoning), EternalBlue (MS17-010), WinRM brute-force
- **Impact:** Full AD takeover, ransomware deployment path, complete credential exposure
- **Reference:** `infrastructure-vapt-ad-compromise.html`

### 3. **Investment Holding Company — 6-Month VAPT Retest**
- **Scope:** 101-host flat network, 7 external assets, Active Directory
- **Focus:** Baseline correlation, remediation validation, regression testing
- **Results:** 8 findings closed, 1 high finding still open, 22 tracked items
- **Key Techniques:** Network segmentation testing, SMB signing validation, Kerberos pre-auth checks
- **Reference:** `investment-holding-vapt-retest.html`

### 4. **Android & iOS Pentest — CBC Padding Oracle + JWT Extraction (Fintech)**
- **Scope:** Full-spectrum mobile security assessment
- **Critical Finding:** CBC padding oracle (encryption flaw) confirmed at runtime
- **Key Technique:** Bearer JWT extracted from memory using Frida instrumentation
- **Total Findings:** 27 (5 High/Critical)
- **Platforms:** 2 (Android + iOS)
- **Reference:** `mobile-pentest-android-ios.html`

### 5. **Live JWT Extracted at Runtime — Fintech Mobile & API Pentest (Android)**
- **Scope:** Static + dynamic security assessment
- **Key Finding:** Live Bearer JWT extracted from app memory via Frida
- **Impact:** CVSS 7.3, authentication bypass path, API compromise
- **Total Findings:** 18 (3 High)
- **Tools:** MobSF, Frida, Burp Suite
- **Reference:** `mobile-api-pentest-android.html`

### 6. **ISO 27001:2022 Lead Auditor Training — Competence-Based**
- **Duration:** 3 days, 18 hours, classroom intensive
- **Participants:** 4 (Kropmann and Seamless Technologies)
- **Curriculum:** 40% theory + 60% practical application
- **Progression:** ISMS foundations → risk assessment → audit planning → role-play execution
- **Use Cases Covered:** 7
- **Role-Play Days:** 3
- **Reference:** `iso-27001-lead-auditor-training.html`

---

## Technical Skills & Tooling

### Penetration Testing & Vulnerability Assessment
- **Network Recon:** Nmap, Nessus, Subfinder, Amass
- **Web Application:** Burp Suite Pro, SQLMap, ffuf, Nuclei, Gobuster
- **Active Directory:** CrackMapExec, BloodHound, GetNPUsers.py, secretsdump.py, Impacket, Responder
- **Exploitation:** Metasploit, Zerologon PoC, PetitPotam, PrintNightmare, EternalBlue
- **Mobile:** MobSF, Frida, APKtool, Jadx, Wireshark
- **Cloud & API:** Postman, Wfuzz, theHarvester

### Standards & Frameworks
- **OWASP Top 10 (2021)** — Web application security
- **MASVS** — Mobile application security verification
- **MITRE ATT&CK** — Adversary tactics, techniques, procedures
- **PTES** — Penetration Testing Execution Standard
- **ISO 27001:2022** — Information security management
- **CVSS v3.1** — Vulnerability severity scoring

### Methodologies
- Black-box testing (external attacker perspective)
- Grey-box testing (insider with limited knowledge)
- Active penetration testing (exploitation-focused)
- Passive vulnerability assessment (scanning & analysis)
- Retest validation (remediation correlation)
- Red team exercises (multi-stage attack chains)

---

## Certifications & Qualifications

- **CompTIA Security+** — Foundational security knowledge
- **CEH (Certified Ethical Hacker)** — LinkedIn Learning
- **(ISC)² CC** — Certified in Cybersecurity
- **AWS Academy** — Cloud security foundations
- **ISO/IEC 27001** — Lead Implementer
- **ISO/IEC 27032** — Cybersecurity governance
- **DHS CISA** — Industrial Control Systems Cybersecurity
- **Cisco Jr. Cybersecurity Analyst** — Threat analysis & response

---

## Engagement Standards

✓ **Formal Authorization** — All engagements conducted under written scope & authorization  
✓ **NDA Compliance** — Client identities, infrastructure details, and sensitive data redacted  
✓ **Ethical Conduct** — No unauthorized access, no production systems harmed  
✓ **Documentation** — CVSS v3.1 scoring, OWASP/CWE/CVE mapping, proof-of-concept evidence  
✓ **Remediation Roadmaps** — Prioritized by severity with implementation guidance  
✓ **Retesting** — Follow-up validation engagements to confirm fixes  

---

## Contact & Next Steps

**Oluwatobi Aladetuyi**  
Penetration Tester · Lead Auditor · Security Trainer  
PSE Ltd, Lagos, Nigeria

📧 Email: [available on portfolio site]  
💼 LinkedIn: [available on portfolio site]  

---

**Disclaimer:** All case studies are based on real engagements. Client identities, financial figures, and operational details have been modified or redacted to comply with confidentiality agreements and data protection regulations (NDPR, GDPR, etc.). The findings, techniques, and methodologies are real and documented with proof-of-concept evidence.
