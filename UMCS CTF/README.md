# UMCS CTF 2026

**Event:** UMCS CTF 2026

**Date:** [25–26 April 2026](https://umcybersec.site/) (Online Preliminary Round)

**Team:** USM B!4WaK5

**Team members:** [adrianchx](https://github.com/adrianchx), [SelinaTan](https://github.com/SelinaTan05), [Hooiqi](https://github.com/Hooiqi)

These are our team's writeups from UMCS CTF 2026. Each challenge is grouped by category, with the solver listed at the start of the writeup.

## Challenge Index

| Category | Challenge | Solved by | Main technique |
| --- | --- | --- | --- |
| Misc | [Cloud Whisperer](Misc/Cloud%20Whisperer/README.md) | [@adrianchx](https://github.com/adrianchx) | Base64 decoding |
| Web | [I-DO The Veiled Vow](Web/I-DO%20The%20Veiled%20Vow/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | ZIP known-plaintext attack |
| Web | [REDISTRIBUTE](Web/REDISTRIBUTE/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | Local file read |
| Crypto | [The Hexed Protocol](Crypto/The%20Hexed%20Protocol/README.md) | [@Hooiqi](https://github.com/Hooiqi) | Password mask attack |
| Forensics | [Shadow Ops](Forensics/Shadow%20Ops/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | DNS fragment reassembly |
| Crypto | [Phantom Anthem of DTC](Crypto/Phantom%20Anthem%20of%20DTC/README.md) | [@adrianchx](https://github.com/adrianchx) | Audio cancellation |
| Crypto | [Makmal Buta, UM](Crypto/Makmal%20Buta%2CUM/README.md) | [@Hooiqi](https://github.com/Hooiqi) | Mersenne Twister state recovery |
| Crypto | [Ghost in the Radio](Crypto/Ghost%20in%20the%20Radio/README.md) | [@Hooiqi](https://github.com/Hooiqi) | Rolling XOR |
| DFIR | [Metamon1](DFIR/Metamon1/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | Ransom note analysis |
| DFIR | [Metamon2](DFIR/Metamon2/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | Browser history analysis |
| DFIR | [Metamon3](DFIR/Metamon3/README.md) | [@SelinaTan05](https://github.com/SelinaTan05) | Batch script analysis |

*Cloud Whisperer's Misc classification is based on the supplied solution; its official competition category has not been confirmed.*

## Layout

```text
UMCS CTF/
├── README.md
├── Misc/
│   └── Cloud Whisperer/
├── Web/
│   ├── I-DO The Veiled Vow/
│   └── REDISTRIBUTE/
├── Forensics/
│   └── Shadow Ops/
├── Crypto/
│   ├── The Hexed Protocol/
│   ├── Phantom Anthem of DTC/
│   ├── Makmal Buta,UM/
│   └── Ghost in the Radio/
└── DFIR/
    ├── Metamon1/
    ├── Metamon2/
    └── Metamon3/
```

Each challenge folder contains a `README.md` and an `images/` directory. Images are numbered from `image1.png` within each challenge.
