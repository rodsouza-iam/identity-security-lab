# Authentication Security

## Overview

This section documents the authentication experiments implemented in the Microsoft Entra ID lab.

The objective was to move beyond password-based authentication and explore how stronger authentication methods can be introduced, registered, and used within identity-security scenarios.

The work in this section focuses particularly on phishing-resistant authentication and the relationship between authentication methods, Microsoft Entra authentication policies, Conditional Access, and privileged access.

## Areas Explored

The authentication work includes:

- Microsoft Entra Authentication Methods
- Passkeys (FIDO2)
- Windows Hello for Business
- Authentication registration
- Registration campaigns
- Authentication strengths
- Phishing-resistant authentication

These controls later became important components of the Conditional Access and Privileged Identity Management scenarios documented elsewhere in the lab.

## Documentation Scope

Detailed pages in this section document the authentication methods and registration experiences that were configured and tested.

The documentation distinguishes between:

- authentication methods enabled in the tenant;
- methods actually registered by test identities;
- authentication experiences that were successfully validated;
- authentication requirements enforced through Conditional Access; and
- interactions observed during privileged-access scenarios.

Conditional Access policy design and PIM activation are documented separately so that this section remains focused on the authentication layer itself.
