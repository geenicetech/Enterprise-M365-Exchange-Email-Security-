# Exchange Online Email Security Policy Summary

---

## Purpose

This document summarizes the email security policies implemented in Exchange Online to protect the organization from phishing, malware, spoofing, and malicious content.

---

## Policy Overview

### Anti-Phishing Policy
**Objective:**  
Detect and block phishing attempts and impersonation attacks.

**Key Controls:**
- User and domain impersonation protection
- Mailbox intelligence enabled
- Quarantine action for detected threats

---

### Anti-Malware Policy
**Objective:**  
Prevent malware delivery via email attachments.

**Key Controls:**
- Malware detection enabled
- Common attachment type filtering
- Quarantine action for infected messages

---

### Safe Links Policy
**Objective:**  
Protect users from malicious URLs in email and Office apps.

**Key Controls:**
- Time-of-click URL scanning
- Protection applied to email and Office documents
- Blocks access to malicious links

---

### Safe Attachments Policy
**Objective:**  
Prevent delivery of malicious attachments.

**Key Controls:**
- Dynamic delivery enabled
- Attachments detonated before full access
- Malicious files blocked or delayed

---

### Email Authentication (SPF, DKIM, DMARC)
**Objective:**  
Prevent domain spoofing and improve email trust.

**Key Controls:**
- SPF configured for authorized sending sources
- DKIM enabled for cryptographic message signing
- DMARC configured in enforcement mode with a quarantine policy

---

## Governance & Best Practices

- Defense-in-Depth Strategy: Implementing layered security controls to eliminate single points of failure.
- Active Threat Mitigation: Utilizing DMARC Quarantine to isolate unauthenticated traffic while maintaining mail visibility.
- Continuous Policy Optimization: Setting a routine to update our defenses as email threats change.

---

## Review & Maintenance

- Monitor Defender alerts and reports
- Review quarantine trends
- Adjust policies based on threat patterns
- Periodically review email authentication records
