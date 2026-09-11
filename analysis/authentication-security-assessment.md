# Student Authentication Security Assessment

## Executive Summary

Student accounts can provide access to email, coursework, academic records, financial information, and other sensitive resources. Because compromise of a student account can expose multiple systems and types of information, authentication controls should provide strong security while remaining practical for students to use.

This assessment evaluates a password-and-multifactor authentication (MFA) approach and compares it with alternative authentication methods. The analysis considers security, usability, account recovery, phishing resistance, and user guidance.

The assessment concludes that password-and-MFA authentication provides a stronger baseline than passwords alone, but organizations can further reduce authentication risk by encouraging long, unique passwords, supporting password managers, strengthening MFA options, improving account-recovery guidance, and moving toward phishing-resistant authentication when feasible.

---

## 1. Current Authentication Approach

The evaluated process uses two primary security controls:

1. A password
2. Multifactor authentication

Requiring an additional authentication factor provides protection beyond a password alone. If an attacker obtains a user's password, the attacker would still need to satisfy the additional authentication requirement before accessing the account.

The process also benefits from step-by-step instructions. Breaking authentication setup into individual steps reduces the amount of information users must process at one time and can make security requirements easier to follow.

However, several risks and usability concerns remain.

---

## 2. Password Security Risks

Users may still create predictable passwords, reuse passwords across multiple accounts, or select passwords that are difficult to remember and manage.

Password reuse is particularly concerning because compromise of credentials at one service can increase the risk to other accounts using the same credentials.

Current NIST guidance emphasizes longer passwords and discourages arbitrary password-composition requirements. Password managers can also help users generate and store unique passwords for different services.

### Recommended Controls

Organizations should:

- Encourage long, unique passwords.
- Support the use of password managers.
- Avoid unnecessarily complex composition rules that encourage predictable patterns.
- Prevent known compromised passwords where appropriate.
- Provide clear password-creation guidance to users.

---

## 3. Multifactor Authentication

MFA strengthens authentication by requiring more than one factor before granting account access.

A password-and-MFA model therefore provides greater protection than password-only authentication.

However, MFA technologies provide different levels of protection.

### Authentication Method Comparison

| Approach | Security | Convenience | Primary Limitation |
|---|---|---|---|
| Password only | Low | High | Password may be stolen, guessed, or reused |
| Password + SMS MFA | Moderate | High | SMS provides weaker protection |
| Password + authenticator app | High | Moderate | Requires access to the registered device |
| Passkey / security key | Very High | High after setup | Initial enrollment may require guidance |

This comparison illustrates an important security principle: implementing MFA is valuable, but the method used affects the level of protection provided.

---

## 4. Phishing Resistance

Traditional passwords are vulnerable to phishing because users can be tricked into entering credentials into fraudulent websites.

Some MFA methods can also be susceptible to phishing or social-engineering attacks.

Phishing-resistant authentication methods provide stronger protection because they reduce an attacker's ability to reuse credentials captured through a fraudulent authentication request.

Security keys and passkeys can provide stronger phishing resistance than passwords or authentication methods based on manually entered verification codes.

### Recommendation

Organizations should work toward phishing-resistant authentication when their systems and users can support it.

Where immediate deployment is not feasible, stronger app-based MFA can provide an intermediate improvement over weaker authentication approaches.

---

## 5. Account Recovery and Availability

Authentication security must also consider what happens when users:

- Lose a registered device
- Replace a phone
- Cannot access their primary MFA method
- Forget a password
- Lose access to a recovery method

Without clear recovery procedures, strong authentication controls can create usability problems or encourage users to seek insecure workarounds.

### Recommended Controls

Authentication instructions should clearly explain:

- How to register backup authentication methods
- How recovery codes should be stored
- What to do when a registered device is lost
- How account recovery works
- How users can contact authorized support when recovery fails

Account recovery should be designed carefully so that the recovery process does not become an easier path for attackers than the normal authentication process.

---

## 6. Security and Usability

Authentication controls are more effective when users understand both **how** to use them and **why** they are necessary.

Security instructions should therefore include:

- Clear numbered steps
- Screenshots where appropriate
- Plain-language explanations
- Troubleshooting guidance
- Recovery procedures
- Explanations of the security purpose behind important controls

This approach can reduce confusion while helping users understand why additional authentication requirements exist.

Security and usability should not be treated as competing goals. Well-designed security controls can strengthen protection while reducing unnecessary user frustration.

---

## 7. Risk and Control Summary

| Identified Concern | Potential Risk | Recommended Control |
|---|---|---|
| Weak or predictable passwords | Account compromise | Long, unique passwords |
| Password reuse | Credential reuse across compromised services | Password manager |
| Password-only authentication | Single-factor compromise | MFA |
| SMS-based MFA | Weaker authentication protection | Authenticator app or stronger method |
| Phishing | Credential theft | Phishing-resistant authentication |
| Lost MFA device | Account lockout or insecure recovery | Backup and recovery procedures |
| Confusing instructions | User error or poor adoption | Clear technical documentation |
| Lack of security context | Reduced user understanding | Explain purpose of controls |

---

## 8. Recommendations

Based on the assessment, the following improvements should be prioritized:

### Priority 1 — Maintain MFA

MFA should remain a baseline control because it provides protection beyond a password alone.

### Priority 2 — Improve Password Practices

Users should be encouraged to use long, unique passwords and password managers rather than relying on predictable password patterns.

### Priority 3 — Strengthen MFA Options

Organizations should support stronger authentication methods such as authenticator applications and move toward phishing-resistant methods when feasible.

### Priority 4 — Improve Recovery Procedures

Users should receive clear instructions for backup authentication and account recovery before a device is lost or an authentication problem occurs.

### Priority 5 — Improve Security Communication

Authentication instructions should explain both the required steps and the security reasons behind them.

---

## Conclusion

Password-and-MFA authentication provides a useful foundation for protecting student accounts, but authentication security can be strengthened further.

Long and unique passwords, password managers, stronger MFA, phishing-resistant authentication, well-designed recovery procedures, and clear user instructions provide complementary layers of protection.

The assessment demonstrates that effective authentication requires more than selecting a technical control. Security teams must also consider usability, recovery, communication, and how users interact with those controls.

---

## Portfolio Context

This analysis is adapted from academic work completed in a University of Maryland Global Campus Technical Writing course. It demonstrates cybersecurity research, security-control evaluation, risk analysis, technical documentation, and the ability to translate professional cybersecurity guidance into actionable recommendations.

It is an educational portfolio project and does not represent an assessment of UMGC's production systems.
