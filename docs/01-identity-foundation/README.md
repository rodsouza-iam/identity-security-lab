# Identity Foundation

## Overview

The identity lab uses a Microsoft Entra ID and Microsoft 365 tenant provided through Microsoft Demo Experiences.

The environment was already provisioned with licensing, users, groups, applications, and sample data. I therefore did not build the tenant or its initial identity population from scratch.

Instead, I used this pre-provisioned environment as the foundation for hands-on identity and security experiments, creating dedicated identities, groups, roles, and configurations where required for specific scenarios.

Throughout this repository, I distinguish between configuration that was already present in the demo environment and changes that I implemented, tested, or deliberately investigated.

## Lab Identities

The Microsoft Demo Experiences tenant was already populated with sample users and groups. In addition to those existing identities, I created dedicated lab identities for specific security, governance, authentication, and application-integration scenarios.

| Identity | UPN | Primary purpose |
| --- | --- | --- |
| Admin Test | `admin.test@romait23.dedyn.io` | Administrative test identity and validation of the `romait23.dedyn.io` custom domain |
| Emergency Access Account | `emergencyadmin@<demo-tenant>.onmicrosoft.com` | Emergency/break-glass administrative identity used in Conditional Access scenarios |
| Google Test | `google.test@romait23.dedyn.io` | Test identity created during exploration of Google Workspace SSO integration |
| LAB Finance Approver | `lab.finance.approver@<demo-tenant>.onmicrosoft.com` | Finance approval persona used in Identity Governance and Separation of Duties testing |
| LAB Finance Creator | `lab.financial.creator@<demo-tenant>.onmicrosoft.com` | Finance creation persona used in Identity Governance and Separation of Duties testing |
| LAB Helpdesk Operator | `lab.helpdesk@<demo-tenant>.onmicrosoft.com` | Helpdesk administrative persona used in RBAC and privileged-access scenarios |
| LAB Security Reader | `lab.securityreader@<demo-tenant>.onmicrosoft.com` | Read-only security persona used in RBAC scenarios |
| User Test | `user.test@romait23.duckdns.org` | Test identity associated with the earlier DuckDNS custom-domain experiment |

These identities represent different personas within the lab rather than a single set of accounts reused for every experiment.

Additional identities already present in the Microsoft Demo Experiences tenant were used where appropriate to implement or validate specific controls. Those identities are documented only within the relevant technical sections and are not included in this inventory.

Detailed role assignments, access policies, authentication requirements, and governance controls are documented within their respective sections rather than in this inventory.

## Work covered in this section

### Custom Domain and Microsoft 365 Integration

Integration of the `romait23.dedyn.io` custom domain across Microsoft Entra ID and Microsoft 365, with external DNS hosted through deSEC and Exchange Online-related DNS configuration.

Topics include:

- Domain registration and verification
- External DNS configuration
- MX, SPF, and Autodiscover
- Custom UPNs
- Exchange Online integration
- UPN and SMTP address considerations

### Identity and RBAC Foundation

Implementation of dedicated groups, administrative roles, and access models for RBAC scenarios using selected lab identities.

This includes:

- Test administrative identities
- Role-assignable groups
- RBAC group design
- Administrative role assignments
- Least-privilege scenarios

These identities and groups later became the foundation for experiments involving PIM, Conditional Access, authentication, and Identity Governance.

## Documentation approach

Detailed pages in this section document:

- Objective
- Architecture and design
- Configuration
- Validation
- Sanitized evidence
- Troubleshooting
- Lessons learned

Where appropriate, screenshots, diagrams, and configuration examples are included to demonstrate the implementation and observed behavior.

Sensitive tenant information, credentials, tokens, secrets, and unnecessary identity information are excluded or sanitized before publication.
