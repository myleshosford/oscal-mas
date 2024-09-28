# OSCAL for MAS Notice FSM-N06 Cyber Hygiene

This repo provides the Monetary Authority of Singapore (MAS) Notice of Cyber Hygiene in the Open Security Controls Assessment Language (OSCAL), a standardised machine-readable format by the US NIST. This notice is provided as an OSCAL catalog with a corresponding OSCAL profile - useful for building automated system security plans (SSPs) and embedding into CI automation jobs. 

## Validation

You can validate that the catalog is in a valid OSCAL format as declared in the documents metadata field using [https://github.com/defenseunicorns/go-oscal/](go-oscal).

```
./go-oscal validate -f mas_cyber_hygiene_catalog.yaml
```

## What's next?

There is so much unlocked within an organisation once policy, standards, requirements, obligations and controls are represented as code. 
- Git Integration: Your policies can be managed using Git, just like software code. This allows for branching, pull requests, and code reviews, ensuring that any updates to policies go through a structured approval process.
- Auditability: Every change to a policy is recorded, complete with timestamps, authors, and reasons for changes. This allows for complete traceability of policy evolution and ensures compliance during audits.
- Change Management: Using pull requests (PRs) to propose policy changes encourages collaboration and thorough review. Teams can comment on and suggest amendments to policies before they are merged into production, reducing errors and ensuring organizational alignment.
- Rollback and Reversion: If a policy change has unintended consequences, it's easy to revert to a previous version, ensuring minimal disruption while maintaining compliance.