# Emirates SkyCargo (emirates-skycargo)

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
