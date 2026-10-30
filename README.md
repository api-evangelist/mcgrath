# McGrath

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

McGrath is one of Australia's largest residential real estate brokerage networks, founded in Sydney in 1988 by John McGrath and operating a mixed company-owned and franchise network of roughly 118 offices across New South Wales, Queensland, the ACT, Victoria and Tasmania. Its business lines span residential sales, property management and rentals, projects and new-development marketing, rural and livestock, an Asia Desk for offshore buyers, and mortgage broking through Oxygen Home Loans. Listed on the ASX in 2015 as McGrath Limited (ASX:MEA), it was acquired in June 2024 by a consortium of Knight Frank Australia and New Zealand's Bayleys for A$95.5m and delisted from the ASX on 28 June 2024. McGrath sits on the demand side of the Australian property value chain: it is a brokerage that publishes listings into the REA Group (realestate.com.au) and Domain portal duopoly, settles transactions over the PEXA electronic conveyancing network, and consumes valuation data from PropTrack and CoreLogic rather than producing any of those rails itself. Its API posture is honestly nil. No developer portal exists — developer., developers., api., docs., feeds., data. and portal. subdomains of mcgrath.com.au all fail to resolve (NXDOMAIN), and /developers, /api, /docs, /api-docs, /openapi.json, /swagger.json, /$metadata and /.well-known/openid-configuration all return HTTP 404. RESO — the only genuinely mandated machine-readable real estate contract anywhere in this study — is a North American standard driven by NAR and MLS membership; it has no Australian counterpart and McGrath has no RESO Web API or Data Dictionary certification, no OData surface, and no Universal Property Identifier usage. The only interoperability standards McGrath demonstrably implements are robots.txt and twelve XML sitemaps; every /.well-known/ document probed — security.txt, openid-configuration, oauth-authorization-server, api-catalog, ai-plugin.json — and /llms.txt return 404. Its robots.txt enumerates twenty crawler groups including GPTBot, ChatGPT-User, OAI-SearchBot, ClaudeBot, PerplexityBot, Google-Extended, CCBot and Bytespider, but under RFC 9309 group-matching rules those named AI agents are disallowed only from Google Maps JS/RPC paths — the /properties/ and /search/ disallow lands solely on User-agent: *, so the listing corpus is nominally open to the named AI crawlers and closed to generic ones, while the properties-buy/sold/rent/leased sitemaps advertise those same URLs. Reachability is the harder gate: www.mcgrath.com.au sits behind a Vercel Security Checkpoint that answers scripted clients with HTTP 429 and a browser challenge on every path, so no unattended agent can read the site regardless of robots.txt. The listing inventory is a marketing asset routed to portals under commercial agreements, not a developer surface.

**Areas:** Real Estate · Australia · Property Listings · Brokerage · Residential Real Estate · Property Management · Rentals · Mortgage

## McGrath on APIs.io

Everything profiled for McGrath is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/mcgrath/](https://apis.io/providers/mcgrath/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Mcgrath Domain Security](https://apis.io/security/mcgrath/mcgrath-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.mcgrath.com.au/)
- [Blog](https://www.mcgrath.com.au/articles)
- [Terms of service](https://www.mcgrath.com.au/terms)
- [Privacy policy](https://www.mcgrath.com.au/privacy)

## API Evangelist rating

**Kin Score 6.3** — minimal · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 44.6 |
| Contract quality | 0.0 |
| Contract governance | 4.5 |
| Operational transparency | 0.0 |
| Developer ergonomics | 1.2 |
| Access clarity | 10.5 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 13.9** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/mcgrath/](https://apis.io/providers/mcgrath/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for McGrath: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/mcgrath/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
