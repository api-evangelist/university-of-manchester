# University of Manchester (university-of-manchester)

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
