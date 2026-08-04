# OpenZeppelin

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

OpenZeppelin is a Web3 security platform providing tools for secure smart contract development, deployment, monitoring, and automation. The platform includes OpenZeppelin Contracts (the industry-standard Solidity library), Defender (a hosted developer security platform), the open-source OpenZeppelin Relayer for transaction relay infrastructure, and OpenZeppelin Monitor for real-time on-chain activity detection.

**Note:** OpenZeppelin Defender (the hosted platform) is sunsetting on July 1, 2026. New sign-ups were disabled on June 30, 2025. Users are migrating to the open-source Relayer and Monitor projects.

## APIs

### OpenZeppelin Defender API
Programmatic access to the Defender security platform for managing smart contract deployments, transaction relaying, automated monitoring, and governance proposals.

- **Base URL:** `https://defender-api.openzeppelin.com/v2`
- **Auth:** JWT tokens via SRP protocol (60-minute expiry)
- **Docs:** https://docs.openzeppelin.com/defender/sdk
- **API Reference:** https://www.api-docs.defender.openzeppelin.com/

**Modules:** Deploy, Proposal, Relay, Action, Monitor, Admin, Networks, Relay-Signer

### OpenZeppelin Relayer API (Open Source)
Self-hosted transaction relay infrastructure for EVM, Solana, and Stellar networks.

- **Base URL:** `http://localhost:8080/api/v1`
- **Auth:** API key (minimum 32 characters)
- **Docs:** https://docs.openzeppelin.com/relayer
- **GitHub:** https://github.com/OpenZeppelin/openzeppelin-relayer

**Endpoints:** Relayers (15 ops), Plugins, Notifications, Signers, Metrics, Health

### OpenZeppelin Monitor (Open Source)
Self-hosted blockchain monitoring service for real-time on-chain event detection and alerting.

- **Metrics Port:** 8081
- **Docs:** https://docs.openzeppelin.com/monitor
- **GitHub:** https://github.com/OpenZeppelin/openzeppelin-monitor

**Notifications:** Slack, Discord, Email, Telegram, Webhooks, Custom Scripts

### OpenZeppelin Contracts API Reference
Solidity library providing secure, modular smart contract components.

- **Docs:** https://docs.openzeppelin.com/contracts
- **API Reference:** https://docs.openzeppelin.com/contracts/5.x/api/access
- **GitHub:** https://github.com/OpenZeppelin/openzeppelin-contracts
- **NPM:** `@openzeppelin/contracts`

## Resources

| Resource | URL |
|----------|-----|
| Website | https://www.openzeppelin.com/ |
| Documentation | https://docs.openzeppelin.com/ |
| GitHub | https://github.com/OpenZeppelin |
| Forum | https://forum.openzeppelin.com/ |
| Blog | https://www.openzeppelin.com/blog |
| Discord | https://discord.openzeppelin.com/ |
| Status | https://status.openzeppelin.com/ |
| Migration Guide | https://docs.openzeppelin.com/defender/migration |

## Rate Limits

| Limit | Value | Scope |
|-------|-------|-------|
| Defender API requests | 100 req/sec (burst 300) | Per API key |
| Relayer transactions | 50 tx/min recommended | Per relayer |
| JWT token lifetime | 60 minutes | Per session |
| Relayer (OSS) requests | 100 req/sec (configurable) | Per instance |
| Relayer (OSS) concurrency | 100 concurrent (configurable) | Per instance |

## Plans

| Plan | Cost | Status |
|------|------|--------|
| Builder (Defender) | Free | Legacy (sunset 2026-07-01) |
| Professional (Defender) | Contact sales | Legacy (sunset 2026-07-01) |
| Enterprise (Defender) | Custom | Legacy (sunset 2026-07-01) |
| Open Source (Self-Hosted) | Free + infra costs | Active |

---

*Maintained by [API Evangelist](https://apievangelist.com)*
