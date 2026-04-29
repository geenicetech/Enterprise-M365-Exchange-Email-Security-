# Exchange Online Email Security Hardening
## Enterprise-Grade Email Protection in Microsoft 365

---

## Project Overview

This project demonstrates the implementation of **layered email security controls** in Microsoft Exchange Online to protect against phishing, malware, malicious links, and domain spoofing.

The objective is to reduce email-based attack risk by hardening default configurations and applying security controls commonly used in medium and enterprise Microsoft 365 environments.

---

## Business Problem

Email remains the **primary attack vector** for most organizations.

Common challenges include:
- Phishing emails impersonating executives or trusted domains
- Malware delivered through attachments
- Malicious links that activate after delivery
- Domain spoofing due to weak email authentication

While Exchange Online provides built-in protection, additional configuration and policy tuning are required to effectively defend against modern email threats.

---

## Solution Implemented

A **defense-in-depth email security model** was implemented using Microsoft Defender for Office 365 capabilities, including:

- Anti-phishing protection
- Anti-malware policies
- Safe Links
- Safe Attachments
- Email authentication (SPF, DKIM, DMARC)

Each layer addresses a different stage of the email attack chain.

---

## Email Security Architecture Flow

Inbound email is processed through multiple security layers before reaching the user mailbox:

1. Email authentication checks (SPF, DKIM, DMARC)
2. Anti-phishing analysis
3. Anti-malware inspection
4. Safe Links (time-of-click protection)
5. Safe Attachments (file detonation)
6. Delivery to mailbox

See diagram:
diagrams/exchange-online-email-security-flow.png

---

## Security Policies Implemented

### Anti-Phishing Policy
- Impersonation protection for users and domains
- Mailbox intelligence enabled
- Suspicious messages quarantined

### Anti-Malware Policy
- Malware detection enabled
- Common attachment types filtered
- Infected messages quarantined

### Safe Links Policy
- Time-of-click protection enabled
- Applied to email and Office applications
- Protection against rewritten malicious URLs

### Safe Attachments Policy
- Dynamic delivery enabled
- Attachments detonated in a secure environment
- Prevents delivery of malicious files

### Email Authentication
- SPF validated for authorized senders
- DKIM enabled for the tenant domain
- DMARC configured in monitoring mode

---

## Validation

Policies were validated by:
- Reviewing policy configuration status
- Verifying enforcement in the Defender portal
- Confirming email authentication settings

Screenshots are included as evidence of configuration.

---

## Security Benefits Achieved

- Reduced phishing and impersonation risk
- Malware blocked before reaching users
- Protection against malicious links and attachments
- Improved sender trust and domain reputation
- Stronger overall email security posture

---

## Tools & Technologies

- Microsoft Defender portal (security.microsoft.com)
- Exchange Online
- Microsoft Defender for Office 365
- Exchange Online Protection (EOP)

---

## Status

✅ Completed  
This project establishes a hardened Exchange Online environment aligned with enterprise email security best practices.
