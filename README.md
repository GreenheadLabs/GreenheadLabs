<div align="center">
  <img src="assets/banner.jpg" alt="Greenhead Labs — private digital treasury" width="100%" />
</div>

<br />

<div align="center">
  <h1>Greenhead Labs</h1>

  <p>
    <b>Private digital treasury company</b><br />
    Wyoming LLC · Est. 2025 · <a href="https://greenhead.io">greenhead.io</a>
  </p>

  <p>
    Building the XRPL economy brick by brick.<br />
    Protocols, payments, and ledger infrastructure.
  </p>

  <p>
    <a href="https://greenhead.io"><img src="https://img.shields.io/badge/Website-greenhead.io-6BB6F0?style=for-the-badge&labelColor=0d0d0d" alt="Website" /></a>
    <a href="https://x402.greenhead.io"><img src="https://img.shields.io/badge/x402-Live_on_XRPL-00d4aa?style=for-the-badge&labelColor=0d0d0d" alt="x402" /></a>
    <a href="https://greenhead.io/did"><img src="https://img.shields.io/badge/Identity-did:xrpl-23292F?style=for-the-badge&labelColor=0d0d0d" alt="DID" /></a>
    <a href="https://x.com/Greenhead_io"><img src="https://img.shields.io/badge/X-@Greenhead__io-1d9bf0?style=for-the-badge&labelColor=0d0d0d" alt="X" /></a>
  </p>

  <p>
    <a href="https://greenhead.io">Website</a>
    · <a href="https://greenhead.io/greenheadlabs">Company</a>
    · <a href="https://x402.greenhead.io">x402</a>
    · <a href="https://greenhead.io/quack-protocol">Quack Protocol</a>
    · <a href="https://greenhead.io/did">DID</a>
    · <a href="https://greenhead.io/Ourteam">Team</a>
    · <a href="https://www.linkedin.com/company/greenhead-labs/">LinkedIn</a>
  </p>
</div>

---

Greenhead Labs LLC is a Wyoming private digital treasury. We run verifiable on-chain identity, treasury credentials, and pay-per-call ledger APIs on the XRP Ledger — with a long-term approach to capital preservation and infrastructure.

This GitHub account publishes **identity and public gateways**. Application source stays private.

> Private company. Not a fund, exchange, or custodian. No investment products, securities, or custodial services.

## Surfaces

| | | |
| :--- | :--- | :--- |
| **[x402](https://x402.greenhead.io)** | Pay-per-request XRPL data and Grok AI. HTTP 402 → pay on-ledger → retry. No accounts or API keys. | [Docs](https://x402.greenhead.io/docs) |
| **[Quack Protocol](https://greenhead.io/quack-protocol)** | Payment coordination for AI-native operations. Request → authorize → settle. Coordination, not custody. | v1.5.89 |
| **[Identity](https://greenhead.io/did)** | W3C `did:xrpl` documents and verifiable credentials for company, agent, and treasury. | [Credentials](https://greenhead.io/credentials) |
| **[Trade Desk](https://greenhead.io/trader)** | Public market context. Information, not instruction. | [Overview](https://greenhead.io/trader) |

Also: [Duck Nest](https://greenhead.io/ducknest) · [Quack Board](https://greenhead.io/quack-board) · [Lab](https://greenhead.io/lab) · [AI](https://greenhead.io/ai)

## x402

Live on XRPL mainnet. Read the catalog, pay `payTo`, retry once with the Payment hash.

```bash
curl -s https://x402.greenhead.io/.well-known/x402
```

1. `GET` the catalog (free). Note `payTo`, `network` (`xrpl:0`), and price.
2. Send that XRP amount, or 0.01 RLUSD, to `payTo`. Wait for validation.
3. Retry with `X-Payment-Txid: <64-hex hash>`. Each hash is single-use.

Agents: [llms.txt](https://x402.greenhead.io/llms.txt) · [OpenAPI](https://x402.greenhead.io/openapi.json) · [Skill](https://x402.greenhead.io/skills/x402/SKILL.md) · [Status](https://x402.greenhead.io/status)

## Identity

Machine-readable. No login required.

| | |
| ---: | :--- |
| Legal name | Greenhead Labs LLC |
| Jurisdiction | Wyoming, United States |
| Entity | Single-member LLC |
| Founded | 2025 |
| Company DID | [`did:xrpl:r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B`](https://dev.uniresolver.io/#did:xrpl:r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B) |
| Identity wallet | [`r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B`](https://xrpscan.com/account/r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B) |
| XRPL TOML | [greenhead.io/.well-known/xrp-ledger.toml](https://greenhead.io/.well-known/xrp-ledger.toml) |
| DID document | [greenhead.io/did.json](https://greenhead.io/did.json) |

[ID](https://greenhead.io/Id) · [Agent](https://greenhead.io/Agent) · [Treasury](https://greenhead.io/Treasury) · [Domain linkage](https://greenhead.io/.well-known/did-configuration.json)

## Start here

| If you want to… | Go here |
| :--- | :--- |
| Read the company | [greenhead.io](https://greenhead.io) · [Profile](https://greenhead.io/greenheadlabs) |
| Call the public API | [x402 catalog](https://x402.greenhead.io/.well-known/x402) |
| Verify who we are | [DID](https://greenhead.io/did) · [TOML](https://greenhead.io/.well-known/xrp-ledger.toml) |
| Meet the team | [Our team](https://greenhead.io/Ourteam) |
| Partnerships / press | [Contact](https://greenhead.io/flight-path) |

## Contact

[greenhead.io/flight-path](https://greenhead.io/flight-path) · [admin@greenhead.io](mailto:admin@greenhead.io) · [legal@greenhead.io](mailto:legal@greenhead.io) · [@Greenhead_io](https://x.com/Greenhead_io) · [LinkedIn](https://www.linkedin.com/company/greenhead-labs/)

Legal notices: [greenhead.io/legal](https://greenhead.io/legal)

---

<div align="center">
  <sub>© 2026 Greenhead Labs LLC · Wyoming · Est. 2025 · greenhead.io</sub><br />
  <sub>Private company. Does not offer investment products, financial services, securities, or custodial services.</sub>
</div>
