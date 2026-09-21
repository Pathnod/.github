<pre align="center">
██████╗  █████╗ ████████╗██╗  ██╗███╗   ██╗ ██████╗ ██████╗
██╔══██╗██╔══██╗╚══██╔══╝██║  ██║████╗  ██║██╔═══██╗██╔══██╗
██████╔╝███████║   ██║   ███████║██╔██╗ ██║██║   ██║██║  ██║
██╔═══╝ ██╔══██║   ██║   ██╔══██║██║╚██╗██║██║   ██║██║  ██║
██║     ██║  ██║   ██║   ██║  ██║██║ ╚████║╚██████╔╝██████╔╝
╚═╝     ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═════╝
</pre>

<div align="center">

### Proof of presence for physical infrastructure

Pathnod turns passing smartphones into anonymous witnesses that verify whether physical devices are really present where they claim to be.

[Explore the project](https://github.com/Pathnod/pathnod) · [Follow on X](https://x.com/Pathnod)

</div>

---

## The problem

Physical infrastructure networks need to know that deployed devices—charging stations, antennas, sensors, and other DePIN hardware—actually exist and operate at their declared location.

GPS data can be spoofed, self-reported information cannot be trusted, and manual inspections do not scale.

## How Pathnod works

1. A nearby smartphone discovers a registered device over Bluetooth.
2. The phone sends a random challenge that only the genuine device can sign.
3. The phone produces a privacy-preserving witness attestation.
4. Independent attestations are aggregated until the verification threshold is reached.
5. The resulting proof is recorded on Solana and the witnesses can be rewarded in USDC.

```text
Physical device  ← BLE challenge →  Anonymous witness
       │                                  │
       └──── signed response ─────────────┘
                          │
                 Independent witnesses
                          │
                          ▼
                 Proof of presence
                          │
                          ▼
                       Solana
```

## What we are building

- A mobile witness application
- A device SDK and simulator
- A privacy-preserving attestation protocol
- Solana programs for verification and rewards
- APIs and dashboards for infrastructure operators

## Current status

Pathnod is currently in its MVP phase.

Our first milestone is a complete end-to-end flow: a simulated physical device answers a Bluetooth challenge, a mobile witness creates an attestation, and the resulting proof of presence is verified on Solana.

## Principles

- **Privacy by design** — witnesses should not need to reveal their identity or movement history.
- **Independent verification** — one device or one witness should never be enough.
- **Open infrastructure** — operators should be able to integrate Pathnod without rebuilding their network.
- **Verifiable incentives** — rewards should follow useful, non-duplicated attestations.

---

<div align="center">
  <strong>Pathnod</strong><br />
  Proof of presence. Built from the path.
</div>