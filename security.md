# Security
This section gives a cyber security risk assessment for the company and recommended security controls.

[Risk Assessment](#risk-assessment) | [Security Controls](#security-controls) | [Plan](./plan.md) | [Network Design](./network.md) | [Cloud Services](./cloud.md) | [Ethics](./ethics.md) | [Reflection](./reflection.md) | [Return to index](./README.md)

---

## Risk Assessment

This section presents a cyber security risk assessment for the proposed network design of Truelec. The purpose of this assessment is to identify key assets, threats, and vulnerabilities within the organisation’s network and to evaluate the potential risks associated with cyber security incidents.

The risk assessment conducted in this project is a mini risk assessment. Due to limited time and available information, only selected stages of a full risk assessment process have been applied. The assessment follows the methodology and spreadsheet template provided in the unit and evaluates risks across multiple information security threat categories.

The scope of the risk assessment includes:
- Headquarters network infrastructure
- Branch office network infrastructure
- On-premise and cloud-hosted application servers
- Wired and wireless network services
- Organisational data assets, including operational, employee, and customer data

Cyber security risks are evaluated with respect to confidentiality, integrity, and availability of information assets. Both technical and organisational vulnerabilities are considered to provide a realistic assessment of the organisation’s security posture.

The detailed risk assessment, including the asset register, risk register, and Threat–Vulnerability–Asset (TVA) matrix, has been completed using the provided spreadsheet template.

[View risk assessment spreadsheet](./risk-assessment.xlsx)

---

## Security Controls

Based on the risk assessment results, customer booking data was identified as one of the highest risk data assets due to its sensitivity and importance to business operations. The following security controls are recommended to reduce the likelihood and impact of identified risks.

### Access Control and Authentication

Strong access control mechanisms should be implemented to restrict access to sensitive systems and data. This includes role-based access control, strong password policies, and multi-factor authentication for critical systems such as the booking application and database servers.

This control reduces the risk of unauthorised access and limits the potential damage caused by compromised user accounts. A potential disadvantage is increased complexity for users during authentication.

---

### Network Security and Traffic Filtering

Network security controls such as firewalls, intrusion prevention systems, and secure VPN configurations should be deployed to protect internal networks from external threats. Traffic filtering rules should be applied to restrict unnecessary inbound and outbound network access.

These controls reduce the likelihood of malware infections, denial of service attacks, and network interception. However, improper configuration may lead to performance issues or accidental service disruptions.

---

### Data Protection and Backup Controls

Sensitive data should be protected using encryption for data at rest and in transit. Regular backups should be performed and securely stored to ensure data can be recovered in the event of data loss, ransomware attacks, or system failures.

This control minimises the impact of data breaches and improves business continuity. The main limitation is the additional storage and management overhead required for maintaining secure backups.

---

Overall, the recommended security controls provide layered protection across people, processes, and technology. Implementing these controls will significantly improve the organisation’s cyber security posture while balancing usability and operational requirements.
