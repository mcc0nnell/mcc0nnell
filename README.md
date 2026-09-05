# Robert McConnell

**Accessible communications • software assurance • open source • systems architecture**

I build systems at the seams between **protocols, execution, evidence, accessibility, and public infrastructure**.

The work keeps converging on two questions:

1. **Can a communications system prove accessible behavior, not merely connectivity?**
2. **Can a software delivery system prove exactly what it built, shipped, and verified?**

> Make the machine path boring. Make the evidence undeniable.

## Current systems

### [Baudot](https://github.com/mcc0nnell/baudot) + [Tilden](https://github.com/mcc0nnell/tilden)

**Baudot** is an open-source proving ground for interoperable accessible real-time communications. It starts with behavior: deterministic **T.140 real-time text** semantics and test vectors, then layers SIP/RFC 4103, WebRTC, gateways, and application integrations on top.

The current harness uses **JAIN SIP** as a glass-box signaling instrument, **Sandia Wiretap** as a controlled network/evidence substrate, and independent implementations as external oracles. Transfer, renegotiation, redundancy, and handoff are judged by preserved evidence rather than signaling success alone.

**Tilden** is the companion project for **federated identity, addressing, discovery, and capability resolution**. Baudot answers *what accessible communication behavior must occur*; Tilden addresses *how endpoints and capabilities are found and resolved across a federation*.

Together they point toward a larger goal: **accessible calling as interoperable public infrastructure rather than a collection of isolated applications**.

### WindAnvil

**WindAnvil** is an independent clean-lab software assurance authority: give it an immutable source object and it returns policy-bound evidence of what was actually proven — **PASS, FAIL, or BLOCKED**.

The model is intentionally separate from the build system under test. Reproducibility, SBOMs, provenance, attestations, policy evaluation, and preserved evidence belong to an independent verification path, not a self-reported green check.

### [HORN](https://github.com/mcc0nnell/horn)

HORN is a visual reasoning environment inspired by Robert E. Horn's mural-scale information maps. The premise is simple: **spatial arrangement is meaning**. Rather than flatten a knowledge structure into pages or cards, HORN treats the map itself as an explorable reasoning surface.

### RUSTBELT

[RUSTBELT](https://github.com/mcc0nnell/scumm3) is my experimental runtime for executable narrative, historical systems, BBS-era interfaces, and strange interactive artifacts. It is also where I test the idea that notebooks, evidence, simulation, and interface objects can move between creative and assurance runtimes without losing provenance.

## Apache contribution trail

[![Iceberg — Release Identity](https://img.shields.io/badge/Apache%20Iceberg-Release%20Identity-informational?style=flat-square)](https://github.com/apache/terraform-provider-iceberg/pull/105)
[![Celix — Reproducible Dependency State](https://img.shields.io/badge/Apache%20Celix-Reproducible%20Dependency%20State-informational?style=flat-square)](https://github.com/apache/celix/pull/845)
[![Camel K — Artifact-Bound Assurance](https://img.shields.io/badge/Apache%20Camel%20K-Artifact--Bound%20Assurance-informational?style=flat-square)](https://github.com/apache/camel-k/pull/6777)
[![Maven Parent — Inherited Release Policy](https://img.shields.io/badge/Apache%20Maven-Inherited%20Release%20Policy-informational?style=flat-square)](https://github.com/apache/maven-apache-parent/pull/597)

I tend to work at **authority boundaries**: release identity, reproducible dependency state, artifact-bound evidence, inherited release policy, consumer verification, and the places where automation has to produce evidence strong enough for someone else to trust.

### Software assurance

A recurring question in this work is: **can a downstream consumer prove that the artifact they received is the artifact the project intended to release?**

- [Apache Camel K #6777](https://github.com/apache/camel-k/pull/6777) — artifact-bound CycloneDX SBOMs, immutable image digests, keyless Cosign attestations, and consumer-side verification.
- [Apache Celix #845](https://github.com/apache/celix/pull/845) — native Conan/CycloneDX SBOM generation built around the dependency graph the project already uses.
- [Apache Maven Parent #597](https://github.com/apache/maven-apache-parent/pull/597) — release-time CycloneDX generation in shared Maven inheritance, with the current upstream discussion focused on evidence that is useful at the release boundary rather than SBOM generation for its own sake.
- [FireCrab #190](https://github.com/SteelCrab/firecrab/pull/190) — fail-closed release evidence: installed-package SBOMs, corresponding-source archives bound by SHA-256, and license inventory checks that refuse to publish incomplete evidence.
- Upstream work also spans [Cloudflare CI](https://github.com/cloudflare/ci/pull/5), [Apache Iceberg Terraform](https://github.com/apache/terraform-provider-iceberg/pull/105), [NIST Metaschema](https://github.com/usnistgov/metaschema-java/pull/428), and Sandia tooling.

The pattern is consistent:

**source → artifact → SBOM → digest → attestation → independent verification → preserved evidence**

## Accessible telecom provenance

I was a **key contributor to the MITRE/FCC ACE portfolio**, a public research stack for accessible telecommunications, relay-service experimentation, real-time text and video, interoperability testing, instrumentation, and operational tooling.

The public [MITRE FCC ACE organization](https://github.com/mitrefccace) includes accessible communications clients, WebRTC and RTT work, ACE Omni, experiment and logging infrastructure, and the earlier ACE Direct platform lineage.

[ACE Omni on Cloudflare](https://github.com/mcc0nnell/ace-omni-cf) continues that laboratory model: controlled communications experiments with runtime-independent fixtures, semantic traces, and replayable evidence. Baudot takes the next step by pulling portable accessibility behavior and interoperability claims into their own explicit test vocabulary.

## Small tools + maps

[Yeet](https://github.com/mcc0nnell/yeet) is a small agent shipping contract: take the shortest compliant path, then prove the remote state actually landed.

[awesome-federal-tech](https://github.com/mcc0nnell/awesome-federal-tech) is a practitioner map for OSCAL, SBOMs, ATO, and experimental infrastructure — repositories you can clone, not slideware.

## Working with

`Git` · `Java` · `TypeScript` · `Rust` · `Go` · `Cloudflare` · `SIP` · `WebRTC` · `T.140` · `RFC 4103` · `JAIN SIP` · `Wiretap` · `SBOM` · `CycloneDX` · `Sigstore` · `OSCAL` · `CI/CD` · `software supply chain` · `telecom` · `accessibility`

## Writing

Recent: [Why Apache Matters: The Infrastructure Beneath the Infrastructure](https://mcc0nnell.org/apache)

More at **[mcc0nnell.org](https://mcc0nnell.org)**.
