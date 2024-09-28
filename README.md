# OSCAL for MAS Notice FSM-N06 Cyber Hygiene

This repository provides the Monetary Authority of Singapore (MAS) Notice of Cyber Hygiene in the Open Security Controls Assessment Language (OSCAL), a standardised machine-readable format by the US NIST. This notice is provided as an OSCAL catalog with a corresponding OSCAL profile - useful for building automated system security plans (SSPs) and embedding into CI automation jobs. 

## Validation

You can validate that the catalog is in a valid OSCAL format as declared in the documents metadata field using [https://github.com/defenseunicorns/go-oscal/](go-oscal).

```
./go-oscal validate -f mas_cyber_hygiene_catalog.yaml
```

## What's next?

There is so much unlocked within an organisation once policy, standards, requirements, obligations and controls are represented as code.

### 1. Version Control: Treating Policy Like Software
- **Git Integration**: Your policies can be managed using Git, just like software code. This allows for branching, pull requests, and code reviews, ensuring that any updates to policies go through a structured approval process.
- **Auditability**: Every change to a policy is recorded, complete with timestamps, authors, and reasons for changes. This allows for complete traceability of policy evolution and ensures compliance during audits.
- **Change Management**: Using pull requests (PRs) to propose policy changes encourages collaboration and thorough review. Teams can comment on and suggest amendments to policies before they are merged into production, reducing errors and ensuring organizational alignment.
- **Rollback and Reversion**: If a policy change has unintended consequences, it's easy to revert to a previous version, ensuring minimal disruption while maintaining compliance.

### 2. Automation of Compliance Validation
- **Continuous Compliance**: By integrating policy-as-code into your CI/CD pipeline, you can automatically validate that all code, infrastructure, and system configurations adhere to organizational policies before they are deployed. For example, if a developer deploys an application, the system could automatically check if security controls (e.g., encryption, access management) are in place.
- **Automated Audits**: Auditing becomes less about manual checks and more about programmatically verifying compliance. Scripts can continuously monitor systems for policy violations and alert teams before issues escalate.
- **Real-Time Enforcement**: Policies can be enforced in real-time, ensuring non-compliant changes are blocked or flagged immediately during build or deployment phases. This minimizes security risks and ensures consistent application of controls across environments.

### 3. Dynamic Policy Customization
- **Context-Aware Policies**: Policies can be dynamically adjusted based on system or environment context (e.g., production vs. development, critical vs. non-critical systems). This allows for flexible policy enforcement while maintaining risk-based controls.
- **Adaptive Policies**: As technology or operational practices evolve, policy changes can be rapidly implemented and enforced across the organization. You can roll out policy updates, such as new security protocols, across all systems and ensure instant compliance with minimal manual intervention.
- **Policy Templates**: Policies-as-code can serve as reusable templates. For instance, if a new cloud environment is spun up, it can inherit security and compliance policies automatically, ensuring it adheres to organizational standards from day one.

### 4. Integration with Existing Tools and Workflows
- **CI/CD Pipeline Integration**: Codified policies can become part of your existing development workflows. By embedding policy checks into your pipelines, you ensure that security and compliance requirements are met before any code reaches production.
- **Policy Linting**: Just like code can be linted to check for formatting or logical errors, policies can be linted to ensure they follow best practices, are syntactically correct, and do not conflict with other organizational policies.
- **Incident Response Automation**: Policies can trigger automated workflows in response to incidents. For example, if a policy requires encryption of customer data, and unencrypted data is detected, the system can automatically isolate the resource and notify relevant teams.

### 5. Enhanced Reporting and Metrics
- **Policy Coverage Analytics**: You can generate reports showing which systems, departments, or applications are compliant with various controls and policies. This gives a clear, measurable view of compliance across the organization.
- **Risk Insights**: By mapping policies and controls to real-time data, you can identify areas where non-compliance is common, helping to prioritize risk mitigation efforts.
- **Dashboards**: Real-time dashboards can provide visibility into policy adherence, control coverage, and any outstanding compliance risks, allowing leadership to make informed decisions quickly.

### 6. Collaboration Across Teams
- **Cross-Functional Input**: Security, development, operations, and compliance teams can collaborate on policies in a shared codebase. This ensures that all teams are aligned on security controls, legal obligations, and best practices.
- **Shared Responsibility**: Codified policies promote a culture of shared responsibility for security and compliance. Engineers, for instance, can be directly involved in implementing and enforcing security policies in their code.
- **Continuous Learning**: With policies as code, teams can implement best practices, learn from one another, and contribute to an evolving knowledge base that benefits the entire organization.

### 7. Incident Response and Disaster Recovery
- **Instant Validation**: After an incident, you can quickly query your codified policies to validate that all required controls were in place at the time of the incident, aiding in root cause analysis and determining whether policy gaps contributed to the breach.
- **Automated Remediation**: For certain types of incidents, codified policies can automatically trigger remediation actions. For example, if a breach is detected, systems might automatically isolate affected resources or trigger a security review.

### 8. Regulatory Alignment and Auditing
- **Automatic Cross-Mapping**: With OSCAL, you can automatically map your internal policies and controls to external regulatory frameworks (e.g., NIST, ISO, GDPR). This simplifies audits and helps ensure that any changes to external regulations are reflected in your internal controls.
- **Instant Compliance Reporting**: Instead of manually collecting evidence for audits, you can instantly generate reports that show how your systems meet compliance standards and regulatory requirements. These reports can be tailored to specific regulatory bodies or requirements, reducing the burden of audits.

### 9. Continuous Improvement and Optimization
- **Policy Effectiveness Tracking**: By treating policies as code, you can measure the effectiveness of different controls. For instance, you can assess whether certain security measures are reducing incidents over time and adjust policies accordingly.
- **A/B Testing for Security Policies**: You could potentially A/B test different policy configurations to see which are more effective at preventing certain types of incidents, allowing for data-driven improvements.
- **Cost vs. Security Balance**: Codified policies can provide insights into the cost of enforcing certain controls (e.g., stricter access management or encryption requirements) and help you balance security with operational efficiency.

### 10. Future-Proofing Your Organization
- **Scalability**: As your organization grows, codified policies can scale with it. Whether adding new cloud environments, onboarding new teams, or integrating new vendors, policies-as-code allow for rapid, scalable enforcement across all systems.
- **Technology Agnostic**: Policies represented in OSCAL are technology-agnostic, meaning they can be applied across various platforms (on-premises, cloud, hybrid) without being tied to a specific vendor or system, ensuring long-term flexibility.
- **Innovative Use Cases**: By leveraging policy-as-code, you open up the possibility for future integrations with AI or machine learning systems that could detect compliance risks or inefficiencies and recommend policy updates proactively.
