# OSINT-Based Threat Intelligence Assessment (openai.com)



> \*\*Project Type:\*\* Defensive OSINT / Cyber Threat Intelligence (CTI)  

> \*\*Target:\*\* openai.com (Public domain footprint)  

> \*\*Assessment Mode:\*\* Passive OSINT only (no scanning, exploitation, or unauthorized access)  

> \*\*Date:\*\* January 2026  

> \*\*Analyst:\*\* Olumide Solanke



\## Executive Snapshot

This repository contains a \*\*defensive OSINT-based CTI assessment\*\* of \*\*openai.com\*\*, demonstrating how public information can be collected and analyzed to understand an organization’s \*\*external exposure\*\*, \*\*reconnaissance surface\*\*, and \*\*phishing/social engineering risk\*\* — aligned to CTI workflows and \*\*MITRE ATT\&CK\*\*.



\*\*Overall security posture (based on passive OSINT):\*\*

\- Strong baseline signals: reputable infrastructure patterns, clean reputation indicators

\- Primary exposure driver: \*\*publicly discoverable identity signals (email patterns / volume)\*\* and publicly indexed content that can support attacker pretexting



---



\## What This Proves (Recruiter Lens)

At a glance, this project demonstrates capability in \*\*real SOC/CTI workflows\*\*:

\- Structured CTI methodology (Planning → Collection → Processing → Analysis → Dissemination)

\- Evidence-based findings with operational relevance

\- Risk assessment + prioritized mitigations

\- MITRE ATT\&CK mapping for detection alignment

\- SOC-ready playbook thinking (triage → validate → contain → prevent)



---



\## Intelligence Objectives

This assessment answers:

\- What public intelligence could adversaries leverage for \*\*reconnaissance\*\*?

\- What identity and infrastructure signals are visible that could support \*\*phishing/BEC/social engineering\*\*?

\- What defensive controls reduce the likelihood/impact of those threats?

\- How do findings align to \*\*MITRE ATT\&CK Reconnaissance\*\* techniques?



---



\## Scope \& Ethical Boundaries

✅ Passive OSINT only  

✅ Public sources only  

❌ No vulnerability scanning, exploitation, credential testing, or intrusion  

❌ No private data access or bypass attempts



See: \*\*SECURITY.md\*\* and \*\*THREAT\_MODEL.md\*\* for responsible-use framing.



---



\## Tools \& Platforms Used

\- \*\*Google Dorks\*\* – indexed content \& portal discovery  

\- \*\*theHarvester\*\* – email/subdomain enumeration (passive sources)  

\- \*\*Shodan\*\* – internet-facing metadata (no active probing)  

\- \*\*Hunter.io\*\* – email pattern discovery \& exposure scale  

\- \*\*Wayback Machine\*\* – historical site content \& legacy footprint context  

\- \*\*VirusTotal\*\* – domain reputation + indicator validation  

\- \*\*OSINT Framework\*\* – structured tool taxonomy  

\- \*\*MITRE ATT\&CK\*\* – technique mapping for standardization



---



\## Key Findings (High-Level)

1\. \*\*Publicly indexed documentation \& authentication workflows\*\* can support attacker pretexting and targeted phishing narratives.  

2\. \*\*Email exposure + consistent naming patterns\*\* increase likelihood of spear-phishing and impersonation attempts (especially executive targeting).  

3\. \*\*Infrastructure signals\*\* indicate modern cloud/CDN delivery with limited obvious insecure exposure in passive datasets.  

4\. \*\*Reputation signals\*\* (passive) indicate the primary domain is widely recognized as legitimate and clean.



> Full detail is in the report PDF.



---



\## Threat Actor Perspective (How Attackers Would Use This)

Adversaries could combine OSINT outputs to:

\- Build verified target lists for spear-phishing / BEC

\- Craft believable lures using real organizational terminology and portals

\- Map dependencies and third-party relationships to support supply-chain themed lures

\- Identify legacy paths from historical archives to attempt opportunistic access (without needing scanning)



---



\## Defender Takeaways (What Matters Operationally)

\- \*\*Identity signals are the biggest risk multiplier\*\*: email pattern + volume can drive targeted phishing.

\- Public content enables \*\*high-confidence social engineering\*\* (legit language, portals, workflows).

\- Maintain \*\*continuous external exposure monitoring\*\* (OSINT hygiene is a control).



---



\## SOC / CTI Skills Demonstrated

\- Threat intelligence requirements \& collection planning

\- OSINT collection, enrichment, and analysis

\- Exposure-to-threat translation (why it matters)

\- Risk rating \& prioritization

\- Writing for both technical and executive audiences

\- MITRE ATT\&CK mapping for detection planning

\- SOC playbook drafting \& response logic



---



\## How This Maps to Real-World SOC Operations

SOC use-cases mirrored here:

\- \*\*Alert triage:\*\* validate suspicious domains/URLs with reputation sources

\- \*\*Brand protection:\*\* detect impersonation and look-alike patterns early

\- \*\*Threat hunting:\*\* search for reconnaissance indicators \& targeting signals

\- \*\*Preventive controls:\*\* DMARC enforcement, phishing-resistant auth, monitoring



See: \*\*SOC\_PLAYBOOK.md\*\*



---



\## MITRE ATT\&CK Coverage Summary

Primary focus: \*\*Reconnaissance (TA0043)\*\*  

See: \*\*mitre\_attack\_mapping.md\*\* (separate file for recruiter clarity)



---



\## Repository Contents

\- `report/` → final report PDF

\- `evidence/` → screenshots and tool outputs (organized by tool)

\- `THREAT\_MODEL.md` → attack paths \& kill chain logic

\- `SOC\_PLAYBOOK.md` → how a SOC would respond

\- `mitre\_attack\_mapping.md` → technique mapping table

\- `SECURITY.md` → scope, reporting, and safe-use statement



---



\## Disclaimer

This is \*\*educational, defensive CTI work\*\* based solely on \*\*public OSINT\*\*.  

No unauthorized access, exploitation, or active scanning was conducted.



