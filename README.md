# University of Manchester (university-of-manchester)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

## Overview

The University of Manchester is a public research university in Manchester, England, and a founding
member of the Russell Group. Its programmable footprint is small, real, and almost entirely
mis-stated by its own domain names.

The University operates **three** machine-readable surfaces of its own. Everything else that looks
like a Manchester API is a **tenancy** — Manchester's data on a supplier's platform, under a
supplier's contract.

## Type

- `x-type`: university
- `x-category`: Public Research University

## Tags

University, Higher Education, Education, Research, United Kingdom, Russell Group, Library, Digital
Collections, IIIF, Identity Federation, Research Data, Research Computing

## Surfaces, by operator

### Institution-operated

- **Manchester Digital Collections — IIIF Presentation API** (`x-operator: institution`) — IIIF
  Presentation 2.1 manifests and collections over the John Rylands Library's digitised manuscripts.
  Base: `https://www.digitalcollections.manchester.ac.uk/iiif`. Contract:
  [openapi/university-of-manchester-iiif-presentation-api-openapi.yml](openapi/university-of-manchester-iiif-presentation-api-openapi.yml)
- **Manchester Digital Collections — IIIF Image API** (`x-operator: institution`) — IIIF Image 2.0
  level 1 tile and derivative service. Base:
  `https://image.digitalcollections.manchester.ac.uk/iiif`. Contract:
  [openapi/university-of-manchester-iiif-image-api-openapi.yml](openapi/university-of-manchester-iiif-image-api-openapi.yml)
- **Shibboleth SAML Identity Provider** (`x-operator: institution`) — entityID
  `https://shib.manchester.ac.uk/shibboleth`, scope `manchester.ac.uk`, published as signed
  machine-readable metadata through the Jisc UK Access Management Federation and eduGAIN. Metadata:
  [authentication/university-of-manchester-saml-idp-metadata.xml](authentication/university-of-manchester-saml-idp-metadata.xml)

### Tenant-operated (real relationship, supplier's contract)

- **Elsevier Pure CRIS** (`x-operator: tenant`) — `pure.manchester.ac.uk` and
  `research.manchester.ac.uk`, both CNAME to `uom-aws.elsevierpure.com`. Live OAI-PMH 2.0 with seven
  metadata formats; REST API gated by an `api-key` header. Manchester's records, Elsevier's contract.
- **Figshare research data repository** (`x-operator: tenant`) — `figshare.manchester.ac.uk`, CNAME
  to `figshare.com`.

### Rejected

- `api.figshare.com/v2` — generic vendor host shared by every Figshare customer. Removed.
- `https://api.server.test/v1` (eScienceLab "Cratey API") — a real OpenAPI 3.0.3 in a University of
  Manchester repository, but its only server is a placeholder. Not a surface.

## Artifacts

- OpenAPI: [openapi/](openapi/) — 2 contracts, with pristine pre-refine copies in [openapi/_original/](openapi/_original/)
- JSON Schema: [json-schema/](json-schema/)
- Examples (probed, verbatim live responses): [examples/](examples/)
- Conformance: [conformance/university-of-manchester-conformance.yml](conformance/university-of-manchester-conformance.yml)
- Authentication: [authentication/university-of-manchester-authentication.yml](authentication/university-of-manchester-authentication.yml)
- Errors: [errors/university-of-manchester-errors.yml](errors/university-of-manchester-errors.yml)
- Lifecycle: [lifecycle/university-of-manchester-lifecycle.yml](lifecycle/university-of-manchester-lifecycle.yml)
- Rules: [rules/university-of-manchester-rules.yml](rules/university-of-manchester-rules.yml)
- Vocabulary: [vocabulary/university-of-manchester-vocabulary.yml](vocabulary/university-of-manchester-vocabulary.yml)
- JSON-LD: [json-ld/university-of-manchester-context.jsonld](json-ld/university-of-manchester-context.jsonld)
- Agentic access: [agentic-access/university-of-manchester-agentic-access.yml](agentic-access/university-of-manchester-agentic-access.yml)
- Plans / Rate Limits / FinOps: [plans/](plans/), [rate-limits/](rate-limits/), [finops/](finops/)

## Education-regime conformance

Probed against the Kin Score `education` regime standards. Conformant and institution-operated:
**shibboleth**, **saml**. Conformant but tenant-operated: **oai-pmh**; partial and tenant-operated:
**orcid**. Not found: scim, lti, oneroster, ed-fi, caliper, qti, datacite, crossref. Evidence for
every line is in [conformance/](conformance/university-of-manchester-conformance.yml).

## Attribution correction — 2026-08-19

This repository previously held **36 OpenAPI documents** titled "University of Manchester &lt;tag&gt;
API", plus 70 collections and every derived schema, example, structure, vocabulary, ruleset, JSON-LD
context, authentication artifact and agentic-access classification built from them. All of it was
**Elsevier's Pure product specification**, which says so about itself:

```yaml
info:
  title: Pure API
  contact:
    email: pure-support@elsevier.com
  version: 5.35.2-2
servers:
- url: /ws/api
```

DNS agrees: `pure.manchester.ac.uk` and `research.manchester.ac.uk` both CNAME to
`uom-aws.elsevierpure.com`. Manchester owns the name; Elsevier runs the machine and wrote the
contract. That is a tenant relationship, recorded as a surface — not a reason to hold the supplier's
specification under the University's slug.

Everything affected is preserved, unreferenced, in
[_vendor-quarantine/](_vendor-quarantine/README.md) so the correction stays auditable. The Kin Score
should fall as a result. The previous score was measuring Elsevier's engineering.

## What is genuinely absent

`data.manchester.ac.uk`, `opendata.manchester.ac.uk`, `api.manchester.ac.uk` and
`developer.manchester.ac.uk` do not resolve. There is no open data portal, no central API host, no
developer portal, no self-service API keys, and no public course, timetable or SIS API — the course
catalog is HTML only. Research IT and the HPC services are documented but not programmable. This is
a correct thin profile of an institution that has not framed its public surfaces as products.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Maintainers

- Kin Lane — kin@apievangelist.com
