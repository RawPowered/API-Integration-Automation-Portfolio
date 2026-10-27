# Evidence scope and delivery status

This repository is a curated index of existing work, not a new integration implementation. Read each linked project as its own product and evidence set.

| Evidence class | Meaning here |
|---|---|
| Public source | Source can be inspected; runtime configuration and production operation still require their own review. |
| Public case documentation | Documents implementation and bounded read-only observations; it does not imply a fresh production transaction. |
| Fictional tour | Shows product direction or interface using fictional records, often with mocked APIs; not an execution result. |
| Historical | Partial configuration or evidence from a past system; not a current working integration. |
| Proposed acceptance | A review procedure or roadmap item, not a test already completed. |


## RawOps Suite evidence added October 26, 2026

122 API source files with contextual model calls, Places caching, communication processing and provider-event handlers. Historical interface captures accompany the source; no new external API transaction is claimed. [Review the role-specific case](RAWOPS-SUITE.md) and [original publication scope](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/PUBLICATION-REVIEW.md).


## Sources and current claims

- [OSINT Dive Deep](https://github.com/RawPowered/osint-dive-deep-v1): public Node/Express, Python/FastAPI and worker source. API contracts and synthetic tests are inspectable. Hosting, provider setup and real customer delivery need operator configuration and separate validation.
- [Flow Fountain for CRMs](https://github.com/RawPowered/flow-fountain-for-crms): public GPL v3 source preview, product release v0.1.2. GoHighLevel/LeadConnector is the original CRM adapter. The product tour uses fictional data and mocked API responses; full live MySQL and external integrations remain unverified in that release.
- [305UGC Showcase](https://github.com/RawPowered/305UGC-Showcase): public documents describe its WordPress-to-Zoho integration. The October 16 read-only review established existing linked CRM Cases, administrative reads and enabled Lead-delivery configuration. No new Lead transaction, full customer journey, cross-customer denial sequence or completed production acceptance is claimed.
- [Zoho CRM Widgets](https://github.com/RawPowered/Zoho-CRM-Widgets) and [Zoho CRM Automations](https://github.com/RawPowered/Zoho-CRM-Automations): public product showcases and fictional tours; commercial implementation source and installation are private.
- [RawGraded](https://github.com/RawPowered/RawGraded): publicly released source illustrates selected PHP API and privacy boundaries. Claims apply only to documented paths; this is not a universal audit of all endpoints.
- [Expert Solar historical case](https://github.com/RawPowered/RawPowered/blob/main/docs/EXPERT-SOLAR.md): preserved partial history of previously functional CRM administration and configuration. The historical system is difficult to demonstrate due to age; missing flows or behaviors are not reconstructed as current proof.

No customer data, credentials, private source, production endpoints or real subject information are copied here. Preparing this portfolio did not touch CRM records or execute or test flows.

## Version and status discipline

Project versions belong to their own repositories. Flow Fountain release v0.1.2 and OSINT Dive Deep product release v1.0.1 are different projects and version contracts. API schemas, worker protocols and engine versions remain component-level identifiers. Do not treat the number in one project name as the release version for another.

[Return to overview](../README.md) · [Remaining evidence and acceptance work](ROADMAP.md)
