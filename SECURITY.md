# Security Policy

We maintain a strict separation between public frontend code and private backend/infrastructure to protect users and partners.

## Reporting a Vulnerability
Email: security@policynow.ca
Please include a clear description, reproduction steps, and impact.

## What is not in this repo
- Secrets, tokens, private keys, service accounts
- Production configs or deployment manifests
- Admin routes, RBAC configs, database credentials/schemas

## Expectations
- Environment variables are set through the hosting provider’s secret store.
- Database access is protected with network rules and RLS/ACLs.
- Admin access requires SSO + 2FA.

## Secret scanning
We run secret scanning and rotate any credential if a leak is suspected.
