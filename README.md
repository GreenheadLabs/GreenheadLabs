<div align="center">
  <img src="assets/banner.jpg" alt="Greenhead Labs — private digital treasury, Wyoming LLC" width="1280" />
  <p>Pay-per-call XRPL APIs and on-chain identity.</p>
  <p>
    <a href="https://x402.greenhead.io/status"><img src="assets/badges/live.png" alt="XRPL Live" width="118" height="28" /></a>
    <a href="https://greenhead.io"><img src="assets/badges/website.png" alt="Website" width="132" height="28" /></a>
    <a href="https://x402.greenhead.io"><img src="assets/badges/x402.png" alt="x402" width="72" height="28" /></a>
    <a href="https://greenhead.io/did"><img src="assets/badges/did.png" alt="did:xrpl" width="96" height="28" /></a>
    <a href="https://x.com/Greenhead_io"><img src="assets/badges/x.png" alt="@Greenhead_io" width="128" height="28" /></a>
    <a href="https://www.linkedin.com/company/greenhead-labs/"><img src="assets/badges/linkedin.png" alt="LinkedIn" width="100" height="28" /></a>
  </p>
</div>

---

Wyoming LLC · Est. 2025 · XRPL identity and HTTP 402 APIs.

## Surfaces

| Product | What it is |
| :--- | :--- |
| **[x402](https://x402.greenhead.io)** | Pay-per-request XRPL data and Grok AI. HTTP 402 → pay on-ledger → retry. No accounts or API keys. [Docs](https://x402.greenhead.io/docs) |
| **[Quack Protocol](https://greenhead.io/quack-protocol)** | Payment coordination for AI-native operations. Request → authorize → settle. Coordination, not custody. |
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

| Catalog | Docs | Skill | Status |
| :--- | :--- | :--- | :--- |
| [llms.txt](https://x402.greenhead.io/llms.txt) | [docs](https://x402.greenhead.io/docs) · [OpenAPI](https://x402.greenhead.io/openapi.json) | [SKILL.md](https://x402.greenhead.io/skills/x402/SKILL.md) | [status](https://x402.greenhead.io/status) |

## Identity

Machine-readable. No login required. Check these files first. This GitHub profile is a DID alias on the company document.

| Check | URL |
| :--- | :--- |
| DID document | [greenhead.io/did.json](https://greenhead.io/did.json) |
| XRPL TOML | [greenhead.io/.well-known/xrp-ledger.toml](https://greenhead.io/.well-known/xrp-ledger.toml) |
| Domain linkage | [greenhead.io/.well-known/did-configuration.json](https://greenhead.io/.well-known/did-configuration.json) |
| Company DID | [r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B](https://dev.uniresolver.io/#did:xrpl:r3E25CzRmwMRNmT15mD3s8tLP9fZHbmN7B) |

Treasury and agent accounts are in the TOML. [ID](https://greenhead.io/Id) · [Agent](https://greenhead.io/Agent) · [Treasury](https://greenhead.io/Treasury)

## Contact

| Channel | Link |
| :--- | :--- |
| Inquiries | [greenhead.io/flight-path](https://greenhead.io/flight-path) |
| Legal | [legal@greenhead.io](mailto:legal@greenhead.io) · [greenhead.io/legal](https://greenhead.io/legal) |
| Security | [SECURITY.md](SECURITY.md) · [legal@greenhead.io](mailto:legal@greenhead.io) |
| X | [@Greenhead_io](https://x.com/Greenhead_io) |
| LinkedIn | [Greenhead Labs](https://www.linkedin.com/company/greenhead-labs/) |

---

<p align="center">
  © 2026 Greenhead Labs LLC · Wyoming · Est. 2025 · greenhead.io<br />
  Private company. Does not offer investment products, financial services, securities, or custodial services.
</p>
