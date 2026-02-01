# SOC Playbook: OSINT-Driven Threats (Phishing / Impersonation / Recon)

## Purpose
Operational response steps for threats suggested by passive OSINT findings:
- Phishing / BEC
- Brand impersonation / look-alike activity
- Recon indicators and suspicious targeting

---

## 1) Detection Sources
- Email security gateway alerts (phishing, spoofing)
- DMARC aggregate & forensic reports
- SIEM sign-in anomalies (impossible travel, new device, risky IPs)
- Threat intel feeds (domain reputation, newly registered domains)
- User reports (SOC mailbox / ticketing)

---

## 2) Triage (0–15 min)
**Validate:**
- Is the sender domain spoofed? Check SPF/DKIM/DMARC results
- Is URL a look-alike? Compare domains, redirects, certificate hints
- Any credential submission indicators? (user reports, proxy logs, browser telemetry)

**Classify severity:**
- Exec impersonation / finance-related = **High**
- Wide distribution campaign = **High**
- Single low-confidence suspicious email = **Medium/Low**

---

## 3) Containment (15–60 min)
- Quarantine/remove message across mailboxes
- Block domains/URLs/IPs at secure web gateway
- Disable compromised accounts; revoke sessions/tokens
- Force password reset + require phishing-resistant MFA for impacted users
- Add IOC watchlist in SIEM

---

## 4) Eradication & Recovery (same day)
- Remove malicious inbox rules / forwarding
- Audit OAuth app grants and third-party access
- Verify mailbox access logs for persistence
- Post-incident user coaching (what happened, what to do next)

---

## 5) Lessons Learned (within 7 days)
- Update detections and blocklists
- Improve DMARC policy toward `reject` where feasible
- Add executive protection controls
- Run targeted phishing simulations based on observed lures
