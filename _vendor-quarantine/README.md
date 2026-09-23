# Vendor-attributed artifacts — quarantined 2026-08-19

Everything in this directory was previously stored under the University of Manchester's own
artifact folders and scored as though the University published it. It does not describe anything
the University of Manchester engineered. It is **Elsevier's Pure product API**, verbatim.

## The evidence

The pristine source, `openapi-original/university-of-manchester-pure-rest.yaml`, says so about
itself (the STEP 0c ownership test — judge a spec by what it declares, never by where it was
fetched):

```yaml
info:
  title: Pure API
  description: "The Pure API provides a secure and complete web services API for using
    and managing research information data in Pure. ..."
  contact:
    email: pure-support@elsevier.com
  version: 5.35.2-2
servers:
- url: /ws/api
```

`info.title` is the vendor's product name. `info.contact.email` is the vendor's support desk.
`info.version` is the vendor's build number. `servers[]` is a relative path with no institutional
host in it at all. Not one field in this contract is Manchester's.

DNS confirms the same conclusion from the other direction:

```
pure.manchester.ac.uk.     CNAME  uom-aws.elsevierpure.com.
research.manchester.ac.uk. CNAME  uom-aws.elsevierpure.com.
```

Manchester owns the name. Elsevier runs the machine and wrote the contract. That is the definition
of a **tenant** relationship, and a tenant relationship is recorded in `apis.yml` as a surface with
`x-operator: tenant` — it is not a reason to hold the vendor's specification under the
institution's slug.

## What was quarantined

| Folder | Count | What it was |
|---|---|---|
| `openapi/` | 36 | One Elsevier Pure contract split by tag by `refine-openapis`, then re-titled "University of Manchester &lt;tag&gt; API". Thirty-six times the apparent footprint for one vendor spec. |
| `openapi-original/` | 1 | The pristine Pure 5.35.2-2 spec the splits came from. |
| `collections/` | 70 | Postman + OpenCollection exports generated from those splits. |
| `examples/` | 4 | Payload examples for Pure entities. |
| `json-schema/` | 4 | Schemas lifted from Pure components. |
| `json-structure/` | 4 | Structures lifted from Pure components. |
| `json-ld/` | 1 | A JSON-LD context whose terms are Pure's entity model. |
| `vocabulary/` | 1 | "University of Manchester Pure CRIS Vocabulary", drawn from the Pure contract. |
| `rules/` | 2 | A Spectral ruleset asserting conformance to the Pure contract. |
| `authentication/` | 1 | Pure's `api-key` header scheme, derived from the Pure spec. |

Everything derived inherits the operator. If the contract is the vendor's, so is every schema,
ruleset, vocabulary and example derived from it.

## Where it belongs

Against Elsevier's own `all/` repo, once. Not against Manchester, and not against the other
institutions running Pure — that is the same failure that put one Figshare contract under
twenty-five university slugs.

Retained rather than deleted so the correction stays auditable. Nothing here is referenced from
`apis.yml`.
