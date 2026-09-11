# Student Authentication Security Assessment

## Overview

This project evaluates a student account authentication process from both a cybersecurity and usability perspective. The assessment compares password and multifactor authentication (MFA) approaches and recommends improvements designed to strengthen account security without creating unnecessary barriers for users.

The project is a portfolio adaptation of academic work completed in a University of Maryland Global Campus Technical Writing course.

## Assessment Objectives

The assessment focuses on:

- Password security and password-management practices
- Multifactor authentication (MFA)
- Phishing-resistant authentication
- Authentication usability
- Account recovery considerations
- Security awareness and user guidance
- Balancing security controls with user experience

## Authentication Approaches Evaluated

| Authentication Approach | Security | Convenience | Primary Limitation |
|---|---|---|---|
| Password only | Low | High | Password may be stolen, guessed, or reused |
| Password + SMS MFA | Moderate | High | SMS provides weaker protection |
| Password + authenticator app | High | Moderate | Requires access to the registered device |
| Passkey / security key | Very High | High after setup | Initial enrollment may require guidance |

## Key Findings

The assessment found that password-and-MFA authentication provides substantially stronger protection than passwords alone, but the strength of MFA depends on the authentication method used.

Important considerations include:

- Long, unique passwords reduce risks associated with predictable or reused credentials.
- Password managers can help users generate and maintain unique passwords.
- MFA provides an additional security layer when passwords are compromised.
- SMS-based MFA provides less protection than stronger authentication methods.
- Authenticator applications can provide stronger protection than SMS-based authentication.
- Passkeys and security keys can provide phishing-resistant authentication.
- Account recovery and backup authentication procedures are important parts of authentication design.
- Security controls should be accompanied by clear instructions explaining both how and why users should follow them.

## Recommendations

Based on the assessment, organizations should consider:

1. Maintaining MFA as a baseline account-security control.
2. Encouraging long, unique passwords and password-manager use.
3. Providing stronger MFA options such as authenticator applications.
4. Moving toward phishing-resistant authentication such as passkeys or security keys when supported.
5. Providing clear account-recovery and backup-authentication instructions.
6. Using screenshots, numbered steps, and troubleshooting guidance during enrollment.
7. Explaining the security purpose of authentication requirements to improve user understanding and compliance.

## Frameworks and Guidance

The original assessment used current cybersecurity guidance from:

- Cybersecurity and Infrastructure Security Agency (CISA)
- National Institute of Standards and Technology (NIST)
- NIST SP 800-63B Digital Identity Guidelines

## Skills Demonstrated

- Cybersecurity research
- Authentication security analysis
- Risk identification
- Security-control comparison
- MFA and password-security concepts
- NIST guidance interpretation
- CISA guidance interpretation
- Security recommendations
- Technical writing
- Technical documentation
- Audience analysis
- Security and usability analysis

## Repository Structure

```text
student-authentication-security-assessment/
├── README.md
├── analysis/
│   └── authentication-security-assessment.md
└── references/
    └── sources.md
## Project Documentation

For a more detailed review of the security assessment and supporting cybersecurity guidance:

- [Full Authentication Security Assessment](analysis/authentication-security-assessment.md)
- [References and Cybersecurity Guidance](references/sources.md)
