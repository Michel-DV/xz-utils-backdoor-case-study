# XZ Utils Backdoor Case Study — v1.0.0

Initial public release of **CASE-002** in the Michel-DV Threat Case Studies series.

This publication reconstructs CVE-2024-3094 from the human trust path through the release-engineering mismatch, malicious build-stage extraction, compromised liblzma artifact, transitive loading into selected OpenSSH servers, runtime symbol redirection and operator-only authentication trigger.

## Included

- maintainer trust / governance analysis
- Git tag vs release-tarball mismatch
- build-time payload staging through opaque test files
- liblzma malicious object injection
- platform and anti-analysis gates
- `sshd → libsystemd → liblzma` dependency reconstruction
- GNU IFUNC / loader-time hooking
- pre-authentication trigger architecture
- ecosystem exposure analysis
- detection and response guidance
- representative MITRE ATT&CK mapping
- original trust-boundary reconstruction
- original detection hypotheses
- safe Red Team / research emulation notes
- primary-source evidence trail

## Publication status

**v1.0.0 is the final analytical edition of CASE-002.** Future changes should be limited to factual corrections, broken references, or material new evidence.

**Author:** @Michel-DV  
**License:** CC BY-NC-ND 4.0  
**Publication date:** 15 September 2026
