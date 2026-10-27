# iso27001-soa-cloudnative-analytics
Practice project: risk-driven ISO/IEC 27001:2022 Statement of Applicability for a fictional cloud SaaS company, with defended control exclusions and alternative measures.

The Scenario
---

Company: CloudNative Analytics Ltd Industry: B2B SaaS - Data Analytics Platform Employees: 85 (fully remote) Infrastructure: 100% cloud (AWS), no physical data centers Customers: 200+ enterprise clients requiring ISO 27001 certification 

Goal: Achieve ISO 27001:2022 certification within 6 months

Business Context
No physical offices (remote-first since founding)
All employees use company-managed laptops
Customer data processed exclusively in AWS (eu-west-1)
No mobile app development
No cryptographic key generation (using AWS KMS)
API-only product (no end-user facing application)
No development outsourcing

Risk Assessment Summary
The company has completed a risk assessment identifying these top risks:

Risk ID	Risk Description	Likelihood	Impact	Risk Level
- R-001	Unauthorized access to customer data	Medium	High	High
- R-002	Employee laptop theft/loss	Medium	Medium	Medium
- R-003	Cloud misconfiguration	High	High	Critical
- R-004	Insider threat	Low	High	Medium
- R-005	Third-party breach (AWS)	Low	Critical	High
- R-006	Business continuity failure	Low	High	Medium


