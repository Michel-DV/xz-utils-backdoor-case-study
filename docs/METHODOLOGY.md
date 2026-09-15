# Methodology

## Scope

This repository reconstructs the XZ Utils backdoor incident (CVE-2024-3094) as a software-supply-chain and trust-boundary case study.

The analysis is limited to publicly available information. It does not claim access to private incident data, law-enforcement attribution, or unpublished victim telemetry.

## Evidence hierarchy

Sources are weighted in the following order:

1. **Original disclosure and project records** — Andres Freund's oss-security disclosure, XZ/Tukaani project records, release notes and review notes.
2. **Distribution advisories** — Debian, Red Hat/Fedora, Kali and other directly affected downstreams.
3. **Foundation / ecosystem guidance** — OpenSSF and OpenJS material on open-source takeover patterns.
4. **Technical reverse engineering** — researchers that directly analyzed the build scripts and binary payload.
5. **Secondary reporting** — used only for context when it does not conflict with stronger evidence.

## Confidence labels

- **Confirmed** — directly supported by primary or first-party technical evidence.
- **Strongly supported** — independently reproduced by multiple technical analyses.
- **Analytical conclusion** — interpretation derived from the documented sequence and controls.
- **Unknown** — not established by public evidence.

## Attribution discipline

`Jia Tan` / `JiaT75` refers to the public project identity/account involved in the incident. The report does not treat the public identity as a verified real-world person and does not assign a government sponsor.

## Safety boundary

The report explains the backdoor architecture, build chain and runtime hooking at a level appropriate for defensive research and incident reconstruction. It intentionally does not provide a deployable malicious liblzma build, attacker private trigger material, or operational instructions for compromising SSH servers.
