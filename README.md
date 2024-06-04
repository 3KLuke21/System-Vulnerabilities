# Vulnerability Assessment Report
**Date:** 4th June 2024

## Introduction
This report provides a comprehensive vulnerability assessment of a remote database server. The company stores critical information on The server, accessed by remote employees worldwide to retrieve data on potential customers. Given the server's public accessibility since the company's launch three years ago, it presents a significant security vulnerability. This report outlines the potential risks and recommended remediation strategies.

## System Description
- **Hardware:** Powerful CPU processor, 128GB memory
- **Operating System:** Latest version of Linux
- **Database:** MySQL database management system
- **Network:** Stable connection using IPv4 addresses
- **Security Measures:** SSL/TLS encrypted connections

## Scope
The scope of this vulnerability assessment covers the current access controls of the system from June 2023 to August 2023. NIST SP 800-30 Rev. 1 was used to guide the risk analysis of the information system.

## Purpose
The database server is crucial for remote employees to access potential customer data, driving sales and customer relationships. Securing this server is imperative to protect sensitive information from unauthorized access, preventing financial and reputational damage. If the server were disabled, business operations would be severely disrupted, hindering employees' ability to access essential data and impacting the company's revenue and customer relationships.

## Risk Assessment

| Threat Source | Threat Event                               | Likelihood | Severity | Risk |
| ------------- | ------------------------------------------ | ---------- | -------- | ---- |
| Hacker        | Obtain sensitive information via exfiltration | 3          | 3        | 9    |
| Employee      | Disrupt mission-critical operations        | 3          | 2        | 6    |
| Customer      | Alter/delete critical information          | 1          | 3        | 3    |

## Approach
The risks were assessed by considering the data storage and management methods of the business. The likelihood of a threat occurrence and the impact of these potential events were weighed against the risks to day-to-day operational needs.

## Remediation Strategy
- **Authentication, Authorization, and Auditing Mechanisms:** Implement strong passwords, role-based access controls, and multi-factor authentication to limit user privileges.
- **Data Encryption:** Use TLS instead of SSL for data in motion.
- **IP Allow-Listing:** Restrict database access to corporate offices to prevent unauthorized users from the internet from connecting to the database.

## Conclusion
Securing the database server is crucial for maintaining the integrity and confidentiality of customer data, ensuring continuous business operations, and safeguarding the company's reputation. Implementing the recommended remediation strategies will significantly mitigate the identified risks and enhance the overall security posture of the information system.
