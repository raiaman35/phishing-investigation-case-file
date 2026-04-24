
# Phishing Investigation Case File

A structured phishing investigation of 5 live, verified phishing URLs 
sourced from PhishTank (active within 2-4 days of analysis). Each sample 
was investigated using industry-standard SOC tools and documented.


## Tools Used
- VirusTotal - URL and IP reputation
- URLScan.io — Safe sandbox detonation
- AbuseIPDB — IP abuse confidence scoring
- WHOIS — Domain registration intelligence
## Samples Analyzed




| Case ID | Category    | Severity              |
| :-------- | :------- | :------------------------- |
| `PHI-001` | `Credential Harvest` | `HIGH` |
| `PHI-002` | `Subscription Scam` | `HIGH` |
| `PHI-003` | `E-commerce Scam` | `HIGH`|
| `PHI-004` | `Credential Harvest`| `HIGH`|
|`PHI-005` | `BEC Impersonation`|`CRITICAL`|




## Key Findings

- **Infrastructure overlap**: PHI-002, PHI-003, PHI-004 all share the 
  same hosting IP (45.74.47.19, SLAYER GROUP LIMITED) - confirming a 
  single threat actor operating a multi-brand phishing campaign
- **Maximum anonymization**: PHI-005 uses triple Cloudflare proxy layering, 
  making the true origin server completely undetectable



## MITRE ATT&CK Techniques Observed
- T1566.002 — Spearphishing Link
- T1583.001 — Acquire Infrastructure
- T1036.005 — Masquerading
- T1090.002 — Proxy
## Files

[Phishing-Case-File.pdf](https://github.com/raiaman35/phishing-investigation-case-file/blob/af321dc0e120c0fbc1eb2f283ec4ec4ba54d70ba/Files/Phishing-Case-File.pdf)

