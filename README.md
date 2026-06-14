# OpenZeppelin

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
