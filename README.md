# Emirates SkyCargo (emirates-skycargo)

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

Emirates SkyCargo is the air cargo division of Emirates Airline, headquartered at Dubai International Airport in the United Arab Emirates, moving general freight, pharmaceuticals, perishables, live animals, valuables, mail and courier traffic across a network of more than 140 destinations on six continents using both freighters and passenger-aircraft bellyhold capacity. In the shipment chain it is the airborne carrier leg sitting between the freight forwarder and the ground handler, and it books almost exclusively through intermediaries rather than shippers directly. Its API posture is advertised but not published: Emirates SkyCargo states on its own Digital Booking Channels page that it offers "a direct API connection to your in-house system" covering booking creation, amendments, cancellations and track and trace, yet there is no developer portal, no API reference, no OpenAPI or AsyncAPI document, no base URL and no self-serve signup anywhere on skycargo.com. Access is obtained only by emailing SkyCargoAPISupport@emirates.com to negotiate a host-to-host connection, by integrating through the CargoWise transport management system, by submitting Freight Forwarding Requests over EDI, or by booking through the WebCargo, CargoAi, Pelicargo and cargo.one marketplaces, which themselves require IATA/CASS accreditation. The one standard the organization documents on its own surface is IATA e-AWB: agents must sign the IATA Multilateral e-AWB Agreement before submitting FWB and FHL cargo messages over EDI messaging. This is an EDI-and-bilateral-integration carrier with a customer-contract portal veneer, not a public API provider.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/emirates-skycargo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/emirates-skycargo/refs/heads/main/apis.yml)

## Tags

- Logistics
- Supply Chain
- United Arab Emirates
- Air Cargo
- Airline
- Freight
- Track and Trace
- EDI
- e-AWB
- Standards

## Timestamps

- **Created:** 2026-07-30
- **Modified:** 2026-07-30

## APIs

### Emirates SkyCargo Host-to-Host API

A direct system-to-system API that Emirates SkyCargo advertises on its own Digital Booking Channels page, described as connecting a freight forwarder's in-house system for real-time instant booking confirmation 24/7, with booking creation, amendments, cancellations and track and trace. No technical contract is published — there is no developer portal, no API reference, no machine-readable specification, no documented base URL, no authentication documentation and no self-serve onboarding. The only published route to access is an email to SkyCargoAPISupport@emirates.com with the subject "Host to Host Connection Via API", which starts a commercial integration project. Listed here because the organization publicly asserts the API exists and names its capabilities, not because a callable contract was found.

- **Human URL:** [https://www.skycargo.com/my-shipments/digital-booking-channels/](https://www.skycargo.com/my-shipments/digital-booking-channels/)
- **Base URL:** none published

#### Tags

- Air Cargo
- Booking
- Track and Trace
- Logistics

#### Properties

- [Documentation](https://www.skycargo.com/my-shipments/digital-booking-channels/)
- [Contact](mailto:SkyCargoAPISupport@emirates.com?subject=Host%20to%20Host%20Connection%20Via%20API)

## Interoperability

A shipment crosses many parties. What this organization publishes, and whether the next party in the chain can speak it:

| Dimension | Finding |
| --- | --- |
| Standard conformance | IATA e-AWB — the IATA Multilateral e-AWB (MeA) Agreement is mandatory before FWB/FHL messages may be sent. No version cited. No ONE Record, Cargo-XML or Cargo-IMP reference on any first-party page. |
| Interface shape | `proprietary-undocumented` |
| Identifier scheme | AWB numbers under IATA airline prefix 176, IATA/CASS agent codes, IATA station codes (DXB hub), plus an internal forwarder-branch mapping. No GS1, UN/LOCODE or customs identifiers. |
| Event model | `polling-only` — track and trace is a read capability of the direct API and the portal. No webhook, subscription, AsyncAPI or status-message vocabulary is published. |
| EDI legacy | First-class. FWB/FHL e-AWB and FFR booking requests both travel over EDI messaging. Onboarding requires a signed IATA MeA Agreement, an e-AWB Configuration Form and an Activation Notice. No VAN/AS2/transport or encoding detail published. |
| Multi-party posture | Publishes to contracted counterparties only — forwarders and marketplaces, never shippers directly. Four gated lanes plus four IATA/CASS-gated marketplaces. |
| Access gate | `commercial-agreement` |

## Common Properties

- [Website](https://www.skycargo.com/)
- [Portal](https://eskycargo.emirates.com/app/offerandorder/)
- [Documentation — Digital Booking Channels](https://www.skycargo.com/my-shipments/digital-booking-channels/)
- [Documentation — e-AWB](https://www.skycargo.com/my-shipments/e-awb/)
- [Support](https://www.skycargo.com/contact-support/)
- [FAQ](https://www.skycargo.com/contact-support/frequently-asked-question-faqs/)
- [Training](https://www.skycargo.com/contact-support/e-skycargo-training/)
- [Terms of Service](https://www.skycargo.com/website-user-agreement/)
- [Privacy Policy](https://www.skycargo.com/privacy/)
- [Blog](https://www.skycargo.com/media-centre)
- [LinkedIn](https://www.linkedin.com/company/emirates-skycargo)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
