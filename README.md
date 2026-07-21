# NexPay — Applied Multi-Cloud Zero Trust Case Study (AWS + Azure)

A security architecture case study for a fictional PCI-scoped B2B FinTech SaaS: threat model,
Zero Trust design (NIST SP 800-207), and a triple-framework control mapping — with a
build-out roadmap into a working lab environment.

**Status: Phase 1 (Design & Planning) complete. Build phases in progress.**
Implemented components land here as they're built; until then, this repo is the design
artifact, and the lab-vs-production scope matrix in the Phase 1 document makes that boundary
explicit.

## What's here

| Piece | Summary |
|---|---|
| **Threat model** | 3 adversary profiles, 7 attack scenarios mapped to MITRE ATT&CK, 5 trust boundaries |
| **ZTA design** | All 7 NIST SP 800-207 pillars mapped to concrete AWS/Azure services, with an enforcement point defined per pillar |
| **Control mapping** | 18 controls, each triple-mapped to a ZT pillar, a MITRE technique, and a PCI DSS v4.0.1 requirement |
| **Scope matrix** | Lab implementation vs. documented production extension, per control |

See [`docs/`](docs/) for the Phase 1 design document.

## Roadmap
- **Phase 2** — AWS 3-tier environment build (VPC isolation, WAF, Cognito, KMS)
- **Phase 3** — Detection & response (reuses components from
  [aws-security-labs](https://github.com/HNCloudSec/aws-security-labs))
- **Phase 4** — Azure identity federation + cross-cloud Sentinel
- **Phase 5–6** — Gap fill, red-team validation

## Related
- [Zero Trust Architecture Reference](https://zta-reference.com) — the general-purpose
  10-layer AWS ZT reference this case study applies to a specific company context.
