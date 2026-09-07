# Public Repository Catalog

This catalog is a structured index of **public repositories owned by [frangelbarrera](https://github.com/frangelbarrera)**. It is intended to make the portfolio easier to understand for human collaborators, technical reviewers, and research systems without overstating project maturity or capabilities.

## Scope

The catalog excludes private repositories and repositories created only as temporary pull-request forks. The `wstg` repository is the sole fork exception because it is the maintained Spanish translation project of the OWASP Web Security Testing Guide. The profile repository itself is excluded from the project catalog because it is the index that presents this information.

## Editorial rules

Repository summaries are restricted to information supported by the repository description, README, and GitHub metadata observed on **2026-09-07**. The catalog does not infer production readiness, regulatory compliance, security guarantees, benchmark superiority, or complete detection coverage. When a project makes an important limitation explicit, that limitation is preserved in the `caveat` field.

`maturity` is deliberately conservative. `not_assessed` means that the catalog does not make a maturity claim. `research`, `curated`, `translation`, `prototype`, and `early_stage` are used only when the repository’s purpose or documentation supports that characterization.

## Data model

Each entry has a stable repository name and URL, a primary category, optional secondary categories, a project type, a restrained summary, technologies, an optional capability list, a conservative maturity label, license information when available, source basis, and a verification date. The JSON Schema in [`repository-catalog.schema.json`](./repository-catalog.schema.json) defines the required structure.

## Categories

The controlled vocabulary is defined in the `taxonomy` object of [`repository-catalog.json`](./repository-catalog.json). The main domains are curated lists and directories, AI-agent infrastructure, OSINT and threat intelligence, network and infrastructure security, ICS/OT and SCADA security, application and AI security, malware and binary analysis, research and evaluations, software-quality tooling, translations and documentation, and software prototypes.

## Verification and maintenance

The catalog is a curated index rather than a live security assessment. Links, capabilities, dependencies, licenses, and external services can change. Entries should be rechecked before being used for procurement, deployment, compliance, incident response, or safety-critical decisions. Update `last_verified` whenever an entry is reviewed, and keep the summary narrower than the repository’s promotional claims.

## Files

- [`repository-catalog.json`](./repository-catalog.json): machine-readable catalog.
- [`repository-catalog.schema.json`](./repository-catalog.schema.json): validation schema.
- [`repository-catalog.md`](./repository-catalog.md): scope and editorial methodology.
