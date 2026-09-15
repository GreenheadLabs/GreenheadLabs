<div align="center">
  <img src="assets/banner.jpg" alt="Greenhead Labs — private digital treasury, Wyoming LLC" width="100%" />
  <p>Pay-per-call XRPL APIs and on-chain identity.</p>
  <p>
    <a href="https://x402.greenhead.io/status"><img src="assets/badges/live.png" alt="XRPL Live" height="28" /></a>
    <a href="https://greenhead.io"><img src="assets/badges/website.png" alt="Website" height="28" /></a>
    <a href="https://x402.greenhead.io"><img src="assets/badges/x402.png" alt="x402" height="28" /></a>
    <a href="https://greenhead.io/did"><img src="assets/badges/did.png" alt="did:xrpl" height="28" /></a>
    <a href="https://x.com/Greenhead_io"><img src="assets/badges/x.png" alt="@Greenhead_io" height="28" /></a>
    <a href="https://www.linkedin.com/company/greenhead-labs/"><img src="assets/badges/linkedin.png" alt="LinkedIn" height="28" /></a>
  </p>
</div>

---

Wyoming LLC · Est. 2025. Verifiable identity, treasury credentials, and HTTP 402 micropayments on the XRP Ledger. Application source stays private.

## Surfaces

| Product | What it is |
| :--- | :--- |
| **[x402](https://x402.greenhead.io)** | Pay-per-request XRPL data and Grok AI. HTTP 402 → pay on-ledger → retry. No accounts or API keys. [Docs](https://x402.greenhead.io/docs) |
| **[Quack Protocol](https://greenhead.io/quack-protocol)** | Payment coordination for AI-native operations. Request → authorize → settle. Coordination, not custody. |
| **[Identity](https://greenhead.io/did)** | W3C `did:xrpl` documents and verifiable credentials for company, agent, and treasury. [Credentials](https://greenhead.io/credentials) |
| **[Trade Desk](https://greenhead.io/trader)** | Public market context. Information, not instruction. |

## x402

[Live on XRPL mainnet](https://x402.greenhead.io/status). Read the catalog, pay `payTo`, retry once with the Payment hash.

```bash
# Free catalog: endpoints, prices, payTo
curl -s https://x402.greenhead.io/.well-known/x402

# Expect HTTP 402, then pay on xrpl:0 and retry
curl -i https://x402.greenhead.io/v1/xrpl/listings
curl -i -H "X-Payment-Txid: <64-hex-hash>" \
  https://x402.greenhead.io/v1/xrpl/listings
```

1. `GET` the catalog (free). Note `payTo`, `network` (`xrpl:0`), and price.
2. Send that XRP amount, or 0.01 RLUSD, to `payTo`. Wait for validation.
3. Retry with `X-Payment-Txid: <64-hex hash>`. Each hash is single-use.

Agents: [llms.txt](https://x402.greenhead.io/llms.txt) · [OpenAPI](https://x402.greenhead.io/openapi.json) · [Skill](https://x402.greenhead.io/skills/x402/SKILL.md) · [Status](https://x402.greenhead.io/status)

## Identity

Machine-readable. No login required. Counterparties should check these three files first. This GitHub profile is listed in the DID `alsoKnownAs`.

| Verify | |
| ---: | :--- |
| DID document | [greenhead.io/did.json](https://greenhead.io/did.json) |
| XRPL TOML | [greenhead.io/.well-known/xrp-ledger.toml](https://greenhead.io/.well-known/xrp-ledger.toml) |
| Domain linkage | [/.well-known/did-configuration.json](https://greenhead.io/.well-known/did-configuration.json) |
| Company DID | [`did:xrpl:r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B`](https://dev.uniresolver.io/#did:xrpl:r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B) |

Treasury and agent accounts are in the TOML. [ID](https://greenhead.io/Id) · [Agent](https://greenhead.io/Agent) · [Treasury](https://greenhead.io/Treasury)

## Contact

| | |
| ---: | :--- |
| Contact | [greenhead.io/flight-path](https://greenhead.io/flight-path) |
| Company | [greenhead.io/greenheadlabs](https://greenhead.io/greenheadlabs) |
| Team | [greenhead.io/Ourteam](https://greenhead.io/Ourteam) |
| Operations | [admin@greenhead.io](mailto:admin@greenhead.io) |
| Legal | [legal@greenhead.io](mailto:legal@greenhead.io) · [greenhead.io/legal](https://greenhead.io/legal) |
| Security | [SECURITY.md](SECURITY.md) · [legal@greenhead.io](mailto:legal@greenhead.io) |
| X | [@Greenhead_io](https://x.com/Greenhead_io) |
| LinkedIn | [Greenhead Labs](https://www.linkedin.com/company/greenhead-labs/) |

---

<div align="center">
  <sub>© 2026 Greenhead Labs LLC · Wyoming · Est. 2025 · greenhead.io</sub><br />
  <sub>Private company. Does not offer investment products, financial services, securities, or custodial services.</sub>
</div>
