# McGrath (mcgrath)

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

McGrath is one of Australia's largest residential real estate brokerage networks, founded in Sydney in 1988 by John McGrath and operating a mixed company-owned and franchise network of roughly 118 offices across New South Wales, Queensland, the ACT, Victoria and Tasmania. Its business lines span residential sales, property management and rentals, projects and new-development marketing, rural and livestock, an Asia Desk for offshore buyers, and mortgage broking through Oxygen Home Loans. Listed on the ASX in 2015 as McGrath Limited (ASX:MEA), it was acquired in June 2024 by a consortium of Knight Frank Australia and New Zealand's Bayleys for A$95.5m and delisted from the ASX on 28 June 2024. McGrath sits on the demand side of the Australian property value chain: it is a brokerage that publishes listings into the REA Group (realestate.com.au) and Domain portal duopoly, settles transactions over the PEXA electronic conveyancing network, and consumes valuation data from PropTrack and CoreLogic rather than producing any of those rails itself. Its API posture is honestly nil.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/mcgrath/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/mcgrath/refs/heads/main/apis.yml)

## Tags

- Real Estate
- Australia
- Property Listings
- Brokerage
- Residential Real Estate
- Property Management
- Rentals
- Mortgage

## Timestamps

- **Created:** 2026-07-26
- **Modified:** 2026-07-26

## APIs

None. No public, documented McGrath API was found. `apis[]` in `apis.yml` is deliberately empty.

## API Posture

### RESO

No RESO presence of any kind. RESO — the Real Estate Standards Organization — is a North American body whose Web API and Data Dictionary certifications are driven by NAR policy and enforced through MLS membership. Australia has no MLS system and no RESO equivalent. McGrath appears nowhere in the RESO certification directory, publishes no OData service root or `$metadata` document, and makes no reference to the RESO Universal Property Identifier (UPI). The honest posture here is **absence**, not "certified but unreachable".

### Access gate

`none-published`. There is no developer agreement, data licence, IDX/VOW equivalent, partner programme or API terms to sign, and no MLS, board or association to join — because no access path of any kind is published. A third party wanting Australian listing or transaction data in machine-readable form goes around McGrath entirely: to REA Group or Domain for listings, PropTrack or CoreLogic for valuation, and PEXA for settlement (PEXA gates its developer portal behind a signed PEXA API Agreement, with OAuth 2.0 or mutual TLS).

### Open data

None. McGrath publishes no open dataset. Its `robots.txt` disallows `/properties/` and `/search/` for every user-agent and explicitly blocks GPTBot, ChatGPT-User, OAI-SearchBot, ClaudeBot, PerplexityBot and others — the clearest available statement that the listing inventory is a marketing asset routed to portals under commercial agreements, not a developer surface.

### Auth model

None published. No API keys, no OAuth 2.0 authorization server, no OpenID Connect discovery document (`/.well-known/openid-configuration` returns HTTP 404), and no SAML member-portal metadata.

### Webhooks, events, SDKs, Postman

None found. No public GitHub organization exists. The absence is itself the finding: McGrath buys technology (CRM, portal syndication, conveyancing) rather than shipping a platform.

## Probes

Every candidate developer host and path was probed on 2026-07-26.

| Target | Result |
| --- | --- |
| `developer.mcgrath.com.au` | NXDOMAIN |
| `developers.mcgrath.com.au` | NXDOMAIN |
| `api.mcgrath.com.au` | NXDOMAIN |
| `docs.mcgrath.com.au` | NXDOMAIN |
| `feeds.` / `data.` / `portal.` / `my.mcgrath.com.au` | NXDOMAIN |
| `https://www.mcgrath.com.au/` | 200 (429 Vercel Security Checkpoint to direct programmatic requests) |
| `https://www.mcgrath.com.au/robots.txt` | 200 |
| `https://www.mcgrath.com.au/developers` | 404 |
| `https://www.mcgrath.com.au/api` | 404 |
| `https://www.mcgrath.com.au/docs` | 404 |
| `https://www.mcgrath.com.au/api-docs` | 404 |
| `https://www.mcgrath.com.au/openapi.json` | 404 |
| `https://www.mcgrath.com.au/swagger.json` | 404 |
| `https://www.mcgrath.com.au/$metadata` | 404 |
| `https://www.mcgrath.com.au/.well-known/openid-configuration` | 404 |

Full provenance, including HTTP status and fetch date for every URL, is recorded in [review.yml](review.yml).

## Common Properties

- [Website](https://www.mcgrath.com.au/)
- [About](https://www.mcgrath.com.au/about-us)
- [Contact](https://www.mcgrath.com.au/contact-us)
- [Offices](https://www.mcgrath.com.au/offices)
- [Agents](https://www.mcgrath.com.au/agents)
- [Careers](https://www.mcgrath.com.au/join-us)
- [LinkedIn](https://au.linkedin.com/company/mcgrath-estate-agents)
- [Facebook](https://www.facebook.com/McGrathEstateAgents/)
- [Robots](https://www.mcgrath.com.au/robots.txt)

## Maintainers

- Kin Lane — kin@apievangelist.com
