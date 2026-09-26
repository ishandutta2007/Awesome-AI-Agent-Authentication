# Awesome-AI-Agent-Authentication

# Top AI Agent Authentication Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on CIAM for Apps & Agents, Machine Identity, OAuth for Agents, Passkeys, SSO & Secure Access to AI Workloads*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Agent Authentication**. These systems authenticate users and non-human identities (agents, workloads, MCP servers)—issuing tokens, enforcing SSO/MFA/passkeys, and scoping permissions so agents act only with appropriate delegated authority.

**Examples** include Descope, WorkOS, Clerk, Auth0, Stytch, Frontegg, Okta CIAM, FusionAuth, Ory, and Hanko (the category leaders).

**Open-source emphasis**: Authentication has excellent open options. **Keycloak**, **Ory**, **Hanko**, **Authentik**, **SuperTokens**, **Zitadel**, and **Logto** power self-hosted CIAM; agent-specific patterns build on OAuth2, SPIFFE, and emerging MCP auth. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Auth0, Okta CIAM](https://auth0.com/)**  
  Enterprise identity platforms widely used for application and API auth—extendable to service accounts and agent-style machine identities.

- **[Clerk, Stytch, Descope](https://clerk.com/)**  
  Developer-friendly CIAM with passkeys, MFA, and modern session management; often used as the user-auth layer in front of AI products and agents.

- **[WorkOS, Frontegg](https://workos.com/)**  
  B2B identity and multi-tenant auth platforms—SSO, directory sync, and enterprise-ready access control for SaaS and agent-powered apps.

- **[FusionAuth, Hanko Cloud](https://fusionauth.io/)**  
  Flexible CIAM with self-host or cloud options; Hanko emphasizes passkeys and passwordless flows.

- **[Ory Network](https://www.ory.sh/)**  
  Managed identity based on the open Ory stack (Kratos, Hydra, Keto)—authn, OAuth2/OIDC, and permissions.

- **[Other commercial agent & CIAM auth platforms](https://auth0.com/)**  
  Additional solutions for non-human identity, MCP OAuth, and fine-grained agent authorization.

## Open-Source GitHub Projects

- **[Keycloak](https://github.com/keycloak/keycloak)**  
  Leading open-source (Apache 2.0) identity and access management—SSO, OIDC/SAML, LDAP federation, service accounts; battle-tested for apps and machine identity.

- **[Ory (Kratos, Hydra, Keto, Oathkeeper)](https://github.com/ory)**  
  Composable open identity stack—user management, OAuth2/OIDC provider, permissions, and zero-trust proxy; ideal foundation for agent token flows.

- **[Hanko](https://github.com/teamhanko/hanko)**  
  Open-source authentication focused on passkeys, 2FA, and modern login; self-host or use Hanko Cloud.

- **[Authentik](https://github.com/goauthentik/authentik)**  
  Flexible open IdP with flows, outposts, and broad protocol support for apps and APIs.

- **[SuperTokens](https://github.com/supertokens/supertokens-core)**  
  Open-source auth with prebuilt and customizable UI—session management and recipes for many app patterns.

- **[Zitadel, Logto, Casdoor](https://github.com/zitadel/zitadel)**  
  Cloud-native and developer-focused open CIAM projects with multi-tenancy, OIDC, and audit-friendly designs.

- **[SPIFFE/SPIRE](https://github.com/spiffe/spire)**  
  Open workload identity framework—cryptographic service identity for machines and agents in dynamic infrastructure.

- **[Better Auth, Stack Auth & TS auth libraries](https://github.com/better-auth/better-auth)**  
  Modern open TypeScript auth libraries used as lightweight alternatives to full IdPs for app and agent backends.

### Additional Strong Open-Source Options

- **Full IdP**: Keycloak or Ory for SSO, OAuth2, and service accounts.
- **Passwordless**: Hanko for passkey-first user auth in front of agent products.
- **Workload/agent identity**: SPIFFE/SPIRE for non-human identity in clusters.
- **Permissions**: Ory Keto or OpenFGA for fine-grained authorization of agent actions.
- **Composable stacks**: Keycloak/Ory for users + client credentials / SPIFFE for agents + short-lived tokens.
- Commercial platforms still lead in polished B2B SSO UX and managed compliance certifications.

**Frameworks for building custom systems**:  
**Keycloak** or **Ory** as the identity core; **Hanko** for passkeys; **SPIFFE/SPIRE** for workload identity.  
Issue short-lived, scoped tokens to agents; prefer OAuth2 client-credentials or delegation patterns over long-lived API keys.  
Commercial CIAM (Auth0, Clerk, WorkOS, Stytch, Descope, etc.) accelerates user auth and enterprise SSO.  
Many AI products use commercial CIAM for humans and open IdPs/SPIFFE for agent and service identity. Fully open stacks are production-viable with operational capacity for IAM.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Agent authentication is high-stakes: leaked tokens or over-privileged agents can cause severe damage. Use least privilege, short token lifetimes, rotation, and audit logs. Emerging MCP and agent-identity standards are still evolving—validate against your threat model.
- Open-source IAM offers control and data residency but requires hardened deployment and updates. Commercial platforms shift operational and compliance burden to the vendor. Neither replaces secure design of agent permissions and tool access.

---

**Made for identity engineers, AI platform teams, and builders securing users and agents.**  
Let's expand open, standards-based authentication for AI agents while recognizing the UX and enterprise depth that leading commercial CIAM platforms deliver.
