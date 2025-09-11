[![DOI](https://zenodo.org/badge/1038390482.svg)](https://doi.org/10.5281/zenodo.16880174)

# REET - the Structural Governance Standard for AI

This repository is the authoritative public record of REET, the Structural Governance Standard for AI.

REET is a complete and verifiable oversight framework. It is defined through fifteen structural tests (Q1–Q15), each with specific questions, pass/fail criteria, and evidence formats. Together, these tests provide a binary outcome: either the safeguards hold, or accountability fails.

The Standard establishes AI governance as a discipline in its own right. Compliance is not treated as a statement of policy or intent but as a structural condition engineered into the system and independently verifiable in operation.

REET integrates:

- A universal taxonomy of structural breaches,
- Operational countermeasures to prevent recurrence,
- Methods of verification that withstand independent audit, and
- Safeguards designed to adapt under changing conditions.

Through these elements, REET sets the enforceable conditions under which trust in AI systems can be established, preserved, and demonstrably proven.

##  The four rights every system must prove

- **Refusal Prevention** - A person must be able to say no without punishment. This means refusal is logged, honoured, and the service continues unchanged. If refusal leads to degraded quality, hidden costs, or is ignored by design, the safeguard has failed.
- **Escalation Suppression** - Every user must be able to challenge a decision to a human with real authority. Escalation must lead out of loops and delays, with a named path, a time-bound SLA, and the ability to overturn outcomes. If escalation routes circle back to automation or powerless staff, the safeguard collapses.
- **Exit Obstruction** - A person must be able to leave without traps or harm. Closure must be real, data must be exportable in open formats, and unrelated services must remain intact. If exit is blocked by hidden fees, circular deletion loops, or retaliation, the system has failed.
- **Traceability Void** - Every decision must be explainable from end to end. That requires a record of the model, the data, and the rule path used. If only dashboards or partial summaries are offered, or if logs vanish when inspected, the safeguard is void.
  
If even one of these rights is denied, accountability fails.

## What REET produces

REET is not a report or a maturity score. It produces binary outcomes and concrete artefacts.

- **Binary results**: each test ends in PASS with evidence or FAIL. There is no middle ground.
- **Breach notes**: when a test fails, REET documents where, how, and why the safeguard collapsed.
- **Comparable signals**: because the same test can be applied anywhere, outcomes can be compared across systems, vendors or jurisdictions.

The outputs are simple, hard, and portable. They can be cited in enforcement, contracts, or disputes without translation.

## The Stages of Accountability

- **Sovereignty & Evidence**: This is the baseline: the minimum conditions of user power. A system must allow refusal without penalty, exit without harm and guarantee that every decision can be traced back to its source. It must also preserve memory so harm cannot be erased or disguised as isolated mistakes. These four rights: to refuse, to leave, to trace and to remember, define sovereignty. Without them nothing else matters.  [Download Sovereignty & Evidence from GitHub](https://raw.githubusercontent.com/russell-parrott/reet/main/inc/Sovereignty-Evidence.pdf)

- **Authority & Fairness**: Once sovereignty is proven the next demand is authority. Users must not be trapped in powerless loops. Escalation must lead to people with real authority to overturn outcomes. Safeguards must be available to all users equally not gated by language, geography or payment tier. Evidence must be durable, verifiable and admissible in disputes. Together these conditions ensure fairness and prevent accountability from being reduced to theatre. [Download Authority-Fairness from GitHub](https://raw.githubusercontent.com/russell-parrott/reet/main/inc/Authority-Fairness.pdf)

- **Integrity & Closure**: At the highest stage, evasions must be shut down completely. Safeguards must work in practice not just on paper. Consent must be genuine and reversible. Remedies must arrive within real deadlines. Metrics must measure harm resolved not performance theatre. Responsibility must follow the chain across vendors and jurisdictions with no loopholes left open. Harm must be recognised in all its forms: financial, emotional, reputational and systemic. Only then can a system claim full integrity. [Download Integrity-Closure from GitHub](https://raw.githubusercontent.com/russell-parrott/reet/main/inc/Integrity-Closure.pdf)
  
## Why this matters

The purpose of REET is not to measure sentiment. It is to create evidence that regulators, buyers and individuals can rely on. 

- Regulators can cite REET failures directly in enforcement orders. 
- Buyers can make contracts contingent on REET passes instead of marketing claims. 
- Boards can demand REET evidence before systems are deployed. 
- Individuals can expose breaches with artefacts that stand up in disputes. 

In every case, REET replaces promises with proof.

## Quick Start

1. Select the relevant stage (Sovereignty, Authority, or Integrity).  
2. Open the corresponding test file in `/tests/`.  
3. Compare the standard against the live system.  
4. Record whether evidence is present and sufficient.  
5. Mark PASS, FAIL, or MISSING PROOF.  

Outputs can be published as a Test Card or attached directly to contracts and regulatory filings.


## What REET is

REET is a public standard of enforceable tests. It is designed to close the gap between what systems claim and what they actually do. It is free to use, copy, and enforce and will always remain open.

## What REET is not

REET is not a maturity model, a grey score, or a survey of opinions. If the safeguard holds, the system passes. If it does not, it fails. There is no in-between.

## Components

| Directory | Description |
|-----------|-------------|
| `/tests/` | Structural test definitions linked to each question and safeguard. |
| `/policy/` | Cross-jurisdiction governance notes and evidence chain considerations. |
| `./SPONSORSHIP.md` | Sponsorship arrangements and conditions for sustaining REET as a public standard. |
| `./` | Publication record and provenance documentation. |

## Design principles

REET is based on the principle that trust in AI cannot be declared — it must be a system condition that is designed and able to be proven in operation.

Each safeguard is mapped to a structural question, with defined criteria for verifying compliance, and anchored to an audit trail capable of withstanding cross-jurisdictional challenges.

## Provenance

REET - the Structural Governance Standard for AI was originated and published by Russell Parrott in 2025.

This repository constitutes the authoritative public record of the doctrine, including its definitions, criteria, and canonical schemas.

DOI: [![DOI](https://zenodo.org/badge/1038390482.svg)](https://doi.org/10.5281/zenodo.16880174)

## Contributing

This repository is an authoritative reference, not an open wiki.  
- Issues may be opened to report errors, request clarification, or log adoption.  
- Pull requests are not accepted for changes to the standard itself.  
- Proposals for extensions or mappings can be raised in `/policy/` as separate notes.  

---

**Author:** Russell Parrott — Author, *Structural Governance Standard for AI*  
**License:** CC BY-ND 4.0 (Attribution required, no derivatives)  
**Repository Description:** Safeguard to halt AI before harm.  
![License: CC BY-ND 4.0](https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg)
![Status: Reference Edition v1.0](https://img.shields.io/badge/Status-Reference%20Edition%20v1.0-blue.svg)
