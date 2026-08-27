# Robert McConnell

**Infrastructure • software assurance • accessibility • open source**

I build systems at the seams between **source code, execution, evidence, and public infrastructure**. My current work centers on software supply-chain assurance, reproducible release evidence, policy-driven automation, and telecom/accessibility systems.

> Make the machine path boring. Make the evidence undeniable.

## Current work

### Software assurance

I’m interested in a simple question: **can a downstream consumer prove that the artifact they received is the artifact the project intended to release?**

- [Apache Camel K #6777](https://github.com/apache/camel-k/pull/6777) — artifact-bound CycloneDX SBOMs, immutable image digests, keyless Cosign attestations, and a consumer-side `TRUST` / `REJECT` verifier for the nightly release path.
- [Apache Celix #845](https://github.com/apache/celix/pull/845) — native Conan/CycloneDX SBOM generation built around the dependency graph the project already uses.
- [Apache Maven Parent #597](https://github.com/apache/maven-apache-parent/pull/597) — move release-time CycloneDX generation into shared Apache Maven inheritance so projects can get the behavior without rebuilding the same machinery locally.
- [FireCrab #190](https://github.com/SteelCrab/firecrab/pull/190) — fail-closed release evidence: installed-package SBOMs, corresponding-source archives bound by SHA-256, and license inventory checks that refuse to publish incomplete evidence.

The pattern is consistent: **source → artifact → SBOM → digest → attestation → verification**.

### Open-source infrastructure

Upstream work across [Cloudflare CI](https://github.com/cloudflare/ci/pull/5), [Apache Iceberg Terraform](https://github.com/apache/terraform-provider-iceberg/pull/105), and [NIST Metaschema](https://github.com/usnistgov/metaschema-java/pull/428).

[Yeet](https://github.com/mcc0nnell/yeet) is a small agent shipping contract: take the shortest compliant path, then prove the remote state actually landed.

[awesome-federal-tech](https://github.com/mcc0nnell/awesome-federal-tech) is a practitioner map for OSCAL, SBOMs, ATO, and experimental infrastructure — repositories you can clone, not slideware.

### Accessibility + telecom

I was a **key contributor to the MITRE/FCC ACE portfolio**, a public research stack for accessible telecommunications, relay-service experimentation, real-time text and video, interoperability testing, instrumentation, and operational tooling.

The public [MITRE FCC ACE portfolio](https://github.com/mitrefccace) spans:

- **Accessible communications clients and media:** [ACE Connect Lite](https://github.com/mitrefccace/aceconnectlite), [ACE Connect Lite public](https://github.com/mitrefccace/aceconnectlite-public), [FCC VATRP](https://github.com/mitrefccace/fcc-vatrp), [VATRP WebRTC](https://github.com/mitrefccace/fcc-vatrp-webrtc), [ACE Quill](https://github.com/mitrefccace/ace-quill), and [ACE Quill Keyboard](https://github.com/mitrefccace/ace-quill-keyboard).
- **Experiment, measurement, and analysis:** [ACE Omni](https://github.com/mitrefccace/ace-omni), [VATRP Log Analysis](https://github.com/mitrefccace/fcc-vatrp-log-analysis), [ACR Demo Agent](https://github.com/mitrefccace/acrdemo-agent), [ACR Demo Provider](https://github.com/mitrefccace/acrdemo-provider), and [Data Logger](https://github.com/mitrefccace/data-logger).
- **Platform and operations:** [Hashconfig](https://github.com/mitrefccace/hashconfig), [Autoinstall](https://github.com/mitrefccace/autoinstall), and the [project site repository](https://github.com/mitrefccace/mitrefccace.github.io).

The earlier ACE platform also included the **ACE Direct, Asterisk, ESB, management portal, ACR/CDR, application server, and user server** components; public mirrors of that generation remain available across GitHub.

[ACE Omni on Cloudflare](https://github.com/mcc0nnell/ace-omni-cf) is my current continuation of that work: rebuilding the laboratory around a runtime-independent experiment model so the same fixtures can produce equivalent semantic traces across Cloudflare, JAIN SLEE, and Elixip, with evidence pinned and replayable.

## Working with

`Git` · `Cloudflare` · `Rust` · `Go` · `Firecracker` · `SBOM` · `CycloneDX` · `Sigstore` · `OSCAL` · `CI/CD` · `software supply chain` · `telecom` · `accessibility`

## Writing

Recent: [Why Apache Matters: The Infrastructure Beneath the Infrastructure](https://mcc0nnell.org/apache)

More at **[mcc0nnell.org](https://mcc0nnell.org)**.
