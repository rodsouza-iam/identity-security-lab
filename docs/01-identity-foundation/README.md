# Identity Foundation

## Overview

The identity lab uses a Microsoft Entra ID and Microsoft 365 tenant provided through Microsoft Demo Experiences.

The environment was already provisioned with licensing, users, groups, applications, and sample data. I therefore did not build the tenant or its initial identity population from scratch.

Instead, I used this pre-provisioned environment as the foundation for hands-on identity and security experiments, creating dedicated identities, groups, roles, and configurations where required for specific scenarios.

Throughout this repository, I distinguish between configuration that was already present in the demo environment and changes that I implemented, tested, or deliberately investigated.

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

Creation of dedicated lab identities and groups for later security scenarios.

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
