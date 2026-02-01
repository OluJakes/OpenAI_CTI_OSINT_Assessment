# \# MITRE ATT\&CK Mapping (Reconnaissance Focus)

# 

# \*\*Tactic:\*\* Reconnaissance (TA0043)

# 

# | Tool / Source | Observation (OSINT) | ATT\&CK Technique | Why It Matters (Threat Use) | Defensive Detection / Control |

# |---|---|---|---|---|

# | Google Dorks | Indexed docs, login-related pages, exposed paths | T1593 Search Open Websites/Domains | Enables profiling, lure accuracy, portal discovery | Monitor indexed content; reduce sensitive exposure; brand monitoring |

# | theHarvester | Email/subdomain enumeration from public sources | T1589 Gather Victim Identity Info | Builds targeting list for spear-phishing and impersonation | DMARC/SPF/DKIM; mailbox protection; alert on suspicious sign-ins |

# | Hunter.io | Email format + large volume discoverable | T1589 Gather Victim Identity Info | Scales targeted phishing/BEC using predictable naming | Executive protection; phishing-resistant MFA; email obfuscation where appropriate |

# | Shodan | Passive internet-facing metadata, TLS/service signals | T1590 Gather Victim Network Info | Helps map dependencies and exposed services without probing | Asset inventory; continuous exposure monitoring; vendor risk review |

# | VirusTotal | Reputation validation + related artifacts | T1593 Search Open Websites/Domains | Helps attacker verify legitimacy or blend-in domains | Use reputation intel for triage; block malicious look-alikes |

# | Wayback Machine | Historical pages, legacy terminology/paths | T1593 Search Open Websites/Domains | Enables realistic pretexting; reveals old URLs/branding | Review archived exposures; decommission legacy endpoints; monitor old paths |

# | OSINT Framework | Structured tool selection by category | T1593 Search Open Websites/Domains | Speeds recon planning and coverage | Use same framework defensively for continuous monitoring |

# 

