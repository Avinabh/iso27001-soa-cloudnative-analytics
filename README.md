# iso27001-soa-cloudnative-analytics
Practice project: risk-driven ISO/IEC 27001:2022 Statement of Applicability for a fictional cloud SaaS company, with defended control exclusions and alternative measures.

The Scenario
---

Company: CloudNative Analytics Ltd Industry: B2B SaaS - Data Analytics Platform Employees: 85 (fully remote) Infrastructure: 100% cloud (AWS), no physical data centers Customers: 200+ enterprise clients requiring ISO 27001 certification 

Goal: Achieve ISO 27001:2022 certification within 6 months

Business Context
---

No physical offices (remote-first since founding)
All employees use company-managed laptops
Customer data processed exclusively in AWS (eu-west-1)
No mobile app development
No cryptographic key generation (using AWS KMS)
API-only product (no end-user facing application)
No development outsourcing

## Risk Assessment and Control Mapping

The organization provided risks identified through its internal risk assessment. I reviewed those risks for relevance to the project scope and mapped them to relevant ISO/IEC 27001:2022 Annex A controls. The accompanying workbook documents my control mappings, risk treatment plan, rationale, and evidence references. The table below summarizes the risks; see the [Risk Controls Traceability workbook](<./Risk Controls Traceability.numbers>) for the detailed mapping.

| Risk ID | Risk Description                     | Likelihood | Impact   | Risk Level |
|---------|--------------------------------------|------------|----------|------------|
| R-001   | Unauthorized access to customer data | Medium     | High     | High       |
| R-002   | Employee laptop theft/loss           | Medium     | Medium   | Medium     |
| R-003   | Cloud misconfiguration               | High       | High     | Critical   |
| R-004   | Insider threat                       | Low        | High     | Medium     |
| R-005   | Third-party breach (AWS)             | Low        | Critical | High       |
| R-006   | Business continuity failure          | Low        | High     | Medium     |


Statement of Applicability (SOA)
---
The project includes a draft ISO/IEC 27001:2022 Statement of Applicability covering all 93 Annex A controls.

| SOA summary                      | Count |
| -------------------------------- | ----: |
| Applicable                       |    91 |
| Not applicable                   |     2 |
| Planned; evidence review pending |    91 |

See the [SOA draft](./CloudNative_Analytics_ISO27001_SoA_Draft.md) for control-by-control justifications, evidence targets, exclusions, and risk traceability.

Key applicability decisions
- Controls 7.1–7.5 and 7.11–7.12 are applicable to the AWS-hosted service and are operated by AWS where relevant. AWS assurance evidence and service coverage still need validation.
- Remote-work and endpoint controls apply to company-managed laptops used by employees.
- 7.6 (Working in secure areas) and 8.30 (Outsourced development) are marked not applicable, subject to the scope and supplier checks described in the SOA.

Draft status
This is a review draft, not a claim of certification or completed implementation. Applicable controls remain marked Planned until implementation evidence is reviewed. Evidence references in the SOA are collection targets, not verified records.
