# Security
This section gives a cyber security risk assessment for the company and recommended security controls.

[Risk Assessment](#risk-assessment) | [Security Controls](#security-controls) | [Plan](./plan.md) | [Network Design](./network.md) | [Cloud Services](./cloud.md) | [Ethics](./ethics.md) | [Reflection](./reflection.md) | [Return to index](./README.md)

---

## Risk Assessment

This risk assessment evaluates the cyber security risks associated with the proposed network design and information systems of Truelec. The assessment focuses on identifying critical assets, relevant threats, existing vulnerabilities, and the potential impact of security incidents on the organisation.

Due to limited information and time constraints, a mini risk assessment approach has been adopted using the risk assessment spreadsheet template provided in the unit. The assessment considers risks across multiple asset categories, including hardware, software, network, data, and people assets, and evaluates risks based on confidentiality, integrity, and availability.

The following key data assets were identified as critical to the organisation:
- Customer booking data
- Employee personal data
- Financial and accounting data
- Operational project data

Multiple information security threat categories were assessed, including unauthorised access, malware and ransomware attacks, data breaches, denial of service attacks, insider threats, network interception, system misconfiguration, and physical security breaches.

Each identified risk was evaluated by assigning likelihood and impact ratings, with overall risk levels calculated using the template’s built-in methodology. The results of the assessment highlight that customer booking data presents the highest overall risk due to its sensitivity and business importance.

[View risk assessment spreadsheet](./risk-assessment.xlsx)

---

## Security Controls

Based on the outcomes of the risk assessment, customer booking data was identified as the highest-risk data asset. The following security controls are recommended to reduce the likelihood and impact of cyber security incidents affecting this data.

### Access Control and Authentication

Strong access control mechanisms should be implemented to ensure that only authorised users can access customer booking data. Role-based access control should be enforced, and multi-factor authentication should be required for all users accessing booking systems, particularly for administrative and remote access.

This control will be implemented on the application servers hosting the booking system and enforced through authentication services and firewall rules. By limiting access based on job roles, the risk of unauthorised access and insider misuse is significantly reduced. Users may experience a slightly longer login process, but this is a reasonable trade-off for improved security.

---

### Network Segmentation and Firewall Enforcement

Customer booking data should be hosted within a dedicated server network segment that is isolated from other internal networks. Strict firewall rules should be applied to allow access only from authorised internal systems and secure VPN connections.

This control will be implemented using the firewall and network segmentation defined in the network design. Network segmentation reduces the ability of attackers to move laterally within the network and limits the potential impact of a security breach. This control has minimal impact on end users when properly configured.

---

### Regular Patching and Malware Protection

All servers hosting the booking application should be regularly patched to address known vulnerabilities. In addition, anti-malware and intrusion prevention tools should be deployed to detect and prevent malicious activity such as malware and ransomware attacks.

This control will be implemented on servers within the server network segment and managed centrally by IT administrators. Regular patching reduces the likelihood of successful exploitation of vulnerabilities, while malware protection helps detect and respond to threats early. Occasional planned maintenance windows may be required, but these can be scheduled to minimise disruption.

---

### Summary

The recommended security controls address the most significant risks identified in the risk assessment by strengthening access control, isolating critical systems, and reducing system vulnerabilities. Together, these controls provide a layered security approach that improves the protection of customer booking data and enhances the overall cyber security posture of the organisation.
