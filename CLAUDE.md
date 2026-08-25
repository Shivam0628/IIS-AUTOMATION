# IIS triage context

## Environment
- Identity: Entra ID, Conditional Access, PIM, passkeys/FIDO2
- Endpoint: Intune (Windows + macOS), Apple Business Manager, Platform SSO
- Mail: Exchange Online, shared mailboxes, forwarding controls
- Privilege: Admin By Request (vendor cert pre-approvals, ML rules)
- SSO: SAML/OIDC integrations
- Tooling: PowerShell 7 + `az rest` delegated auth (never Connect-MgGraph)

## Triage conventions
- Read-first, confirm-before-change discipline
- Cite the Intune/Entra console path, not just the API
- Prefer `az rest` examples for anything Graph-related

## Recurring ticket patterns
(append as they show up: passkey registration failures, MAU loops,
Platform SSO hangs, B2B guest provisioning, OAuth consent grants)
