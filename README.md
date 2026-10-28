# CBUAE Operational Risk Management Regulation: Cyber Crosswalk

A requirement-by-requirement map of the UAE Central Bank's **Operational Risk Management Regulation (Circular C 1/2026, in force 14 September 2026)** to **ISO/IEC 27001:2022**, **NIST CSF 2.0** and the **UAE Information Assurance (IA) Regulation**.

**Headline:** an ISO 27001 certificate fully covers 16 of the 39 requirements mapped here. 11 are partly covered and 12 have no ISO equivalent. The gaps cluster in four places: the Board's role, regulator notification clocks, third-party exit and non-objection, and Critical Operations mapping.

| ISO 27001 coverage | Requirements |
| --- | --- |
| Covered | 16 |
| Partial | 11 |
| Gap | 12 |

## Who this is for

- GRC and risk teams at UAE banks, insurers and other licensed financial institutions (LFIs) checking whether their ISMS meets the new regulation.
- Internal auditors planning a review of Articles 3, 8, 9, 11, 13 and 15.
- Consultants and vendors who sell into UAE financial services and need to know what their clients are now accountable for.

## What is in the repo

| File | What it holds |
| --- | --- |
| [`crosswalk.csv`](crosswalk.csv) | 39 rows. Columns: CBUAE clause, theme, requirement (paraphrased), ISO 27001:2022 clauses and Annex A controls, NIST CSF 2.0 categories, UAE IA control family, ISO coverage rating, gap note, and the evidence an auditor would ask for |
| `CHANGELOG.md` | Version history |
| `LICENSE.md` | CC BY 4.0 |

Open the CSV in Excel or Google Sheets and filter on `iso_coverage = Gap` for the quickest view of where a certified ISMS still falls short.

## The 12 gaps

| ID | CBUAE clause | Why ISO 27001 does not cover it |
| --- | --- | --- |
| XW-04 | Art 2.6 | Fraud risk inside the operational risk framework |
| XW-08 | Art 3.5 | Minimum Critical Operations are defined by the regulator |
| XW-11 | Art 4.2 | The Board itself approves appetite, disruption tolerance and BCP/DR on an annual cycle |
| XW-14 | Art 7.13-7.14 | Independent third-party penetration testing of Critical Functions, reported to the Board |
| XW-22 | Art 8.9 | Master System of Record stored in the UAE, including when outsourced |
| XW-29 | Art 11.10-11.11 | Annual BCP testing with key third parties, severe but plausible scenarios, results to the Board |
| XW-31 | Art 12.5 | Material change: external expert report, 30 days' notice, CBUAE written no-objection |
| XW-33 | Art 13.4-13.5 | Provider resilience at least equivalent; CBUAE non-objection before critical outsourcing |
| XW-36 | Art 15.1 | Notify CBUAE of significant appetite or tolerance breaches |
| XW-37 | Art 15.2 | Notify within 4 hours, summary in 24 hours, notice on return to normal |
| XW-38 | Art 15.3 | Notify within 72 hours of high-risk incidents, using Board-approved criteria |
| XW-39 | Art 16 | Public disclosure of operational risk and resilience information |

## Method

1. Read the regulation on the [CBUAE Rulebook](https://rulebook.centralbank.ae/en/rulebook/operational-risk-management-regulation) (Articles 2 to 4, 7 to 13, 15 and 16), and took the ICT, cyber, resilience, incident, continuity, change, third-party and notification requirements.
2. Paraphrased each requirement. The rulebook text is the authority; this repo does not reproduce it.
3. Mapped each requirement to ISO/IEC 27001:2022 clauses and Annex A controls, NIST CSF 2.0 categories (subcategories only where the match is exact), and UAE IA control families (M1 to M6, T1 to T9).
4. Rated ISO coverage: **Covered** means a well-run ISMS meets it as written; **Partial** means the ISMS meets part of it; **Gap** means ISO has no equivalent.
5. Added the evidence an auditor or the regulator would reasonably ask to see.

## Limits

- The mapping and ratings are the author's professional judgement, not CBUAE guidance. Two practitioners could rate some rows differently.
- UAE IA is mapped at control family level, not individual control.
- Articles 5, 6 and 14 (Senior Management, the operational risk function, Shari'ah non-compliance risk) are out of scope because they are not cyber requirements.
- The regulation took effect on 14 September 2026. CBUAE may issue standards or notices that change the detail. Check the rulebook before relying on any row.
- This is not legal advice.

## Sources

- CBUAE Rulebook: [Operational Risk Management Regulation](https://rulebook.centralbank.ae/en/rulebook/operational-risk-management-regulation) and [Article 8, ICT and Cybersecurity Management](https://rulebook.centralbank.ae/en/rulebook/article-8-ict-and-cybersecurity-management)
- Trowers & Hamlins: [UAE Central Bank raises the bar on operational risk](https://www.trowers.com/insights/2026/september/uae-central-bank-raises-the-bar-on-operational-risk) (issue date 3 February 2026; replaces Circular 163/2018)
- ISO/IEC 27001:2022 and Amendment 1:2024
- NIST [Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) (February 2024)
- UAE Information Assurance Regulation (TDRA, formerly the NESA standard)

## Contributing

Spotted a mapping you would rate differently, or a CBUAE notice that changes a row? Open an issue with the row ID (for example `XW-22`) and your reasoning.

## Author

**Clive (Hakim) Bean**: ISO/IEC 27001 Lead Auditor (GRC Mastery, 2026, Credly-verified). UAE and GCC cyber governance, risk and compliance, with 20 years in IT, network and OT infrastructure. Abu Dhabi.

Licensed under [CC BY 4.0](LICENSE.md).
