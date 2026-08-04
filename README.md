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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Manchester is a public research university in Manchester, England, ranked #31 in the QS World University Rankings 2025. Its public developer/API footprint is research-led: an Elsevier Pure CRIS exposing a live OAI-PMH feed and a documented (key-gated) REST API, the public Research Explorer portal, Shibboleth/SAML federated identity, a Figshare research-data repository, and a small public GitHub organization. No unified, self-service developer portal was found.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-manchester-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, United Kingdom

## APIs

- **Research Explorer OAI-PMH (Pure)** — live OAI-PMH 2.0 metadata harvesting endpoint for the Pure institutional repository. Docs: https://research.manchester.ac.uk/ (base: https://pure.manchester.ac.uk/ws/oai)
- **Pure CRIS REST API** — documented REST (CRUD) API over Elsevier Pure; API-key gated. Docs: https://pure.manchester.ac.uk/ws/api/
- **Research Explorer Portal** — public Pure discovery portal for profiles, outputs, projects and theses. Docs: https://research.manchester.ac.uk/
- **Research Data Repository (Figshare)** — institutional research-data deposits discoverable via the Figshare public API. Docs: https://docs.figshare.com/
- **Shibboleth SAML Identity (SSO)** — federated SAML2 IdP in the Jisc UK Access Management Federation. Docs: https://www.itservices.manchester.ac.uk/

## Plans / Rate Limits / FinOps

- Plans: [plans/university-of-manchester-plans-pricing.yml](plans/university-of-manchester-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-manchester-rate-limits.yml](rate-limits/university-of-manchester-rate-limits.yml)
- FinOps: [finops/university-of-manchester-finops.yml](finops/university-of-manchester-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.manchester.ac.uk/
- GitHub: https://github.com/University-of-Manchester
- LinkedIn: https://www.linkedin.com/school/the-university-of-manchester/
- Developer Portal: https://pure.manchester.ac.uk/ws/api/
- Authentication: https://shib.manchester.ac.uk/

## Notes

All catalogued endpoints were probed on 2026-06-03. The Pure OAI-PMH endpoint returned a valid OAI-PMH 2.0 Identify response ("Pure OAI Repository"); the Pure REST API documentation site, Research Explorer portal, and main website all returned HTTP 200. The Shibboleth IdP host bare root returned HTTP 500 (the SSO flow itself is operational). The Pure REST write API requires an institution-issued API key. No public open-data, course, timetable, or SIS APIs were confirmed. Figshare is third-party-hosted. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
