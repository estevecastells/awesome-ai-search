# AI Search API and MCP Benchmark

**Snapshot:** September 2, 2026

**Edition:** 1.0

**Scope:** Programmatic access to AI-search visibility, citation, response and referral data

This benchmark compares how well AI-search measurement products expose their data and workflows to developers and agents. It measures documented programmatic readiness: capability breadth, interface quality, access, authentication and operational transparency.

It does **not** test the accuracy of the underlying visibility data, sentiment labels, production latency, uptime or return on investment. A high score means that more useful functionality is publicly evidenced and easier to integrate. It is not a general product endorsement.

> **Conflict disclosure:** the maintainer of Awesome AI Search is affiliated with [LLM Pulse](https://llmpulse.ai). The same public-evidence rules and scoring weights were applied to every product. Because the complete ordered leaderboard has not yet been reviewed by an unaffiliated human reviewer, scores are provisional and must not be used for a vendor “#1” claim.

## Quick Results

- **Best documented hosted MCP:** [Peec AI](https://docs.peec.ai/mcp/tools), with 76 fully enumerated tools and a detailed field-level reference.
- **Best open and self-hosted integration layer:** [Canonry](https://github.com/Canonry/canonry), with a progressively loaded 206-tool catalog, a public API and local data ownership.
- **Best API surface in this snapshot:** [Peec AI](https://docs.peec.ai/api/introduction), narrowly ahead of [Scrunch](https://developers.scrunch.com/) after access restrictions are included.
- **Best self-serve API and scan workflow:** [Rank Prompt](https://rankprompt.com/docs/v1/).
- **Best hybrid traditional SEO and AI-search MCP:** [Keyword.com](https://keyword.com/docs/mcp/), although only 6 of its 67 tools are AI-visibility-specific.
- **Deepest enterprise workflow MCP:** [Profound](https://docs.tryprofound.com/mcp/overview), spanning analytics, prompts, agents, projects, documents and knowledge bases.

## Market Snapshot

The market is moving quickly, but programmatic access is no longer rare. CitedIndex's August 2026 census found conventional REST APIs at 53 of 76 AI-visibility products whose API status could be determined. Its MCP census found confirmed MCP support at 27 of 86 software products, with 13 offering access without a high-tier gate. See the [API census](https://citedindex.com/blog/api-access-census-ai-visibility-tools-2026/) and [MCP census](https://citedindex.com/blog/mcp-server-support-ai-visibility-tools-2026/) for the broader market.

## API Leaderboard

The API score rewards public schemas and reference quality (20), raw and aggregate AI-search data (20), engine and metric coverage (15), write/scan/webhook workflows (15), the paired MCP implementation (10), access and pricing transparency (10), and authentication, rate-limit and versioning maturity (10).

Raw operation counts are descriptive, not scoring inputs. A broad API cannot improve its score merely by splitting one workflow into many endpoints.

| Rank | Product | Score | Publicly evidenced API surface | Access | Main limitation |
|---:|---|---:|---|---|---|
| 1 | [Peec AI](https://docs.peec.ai/api/introduction) | **94** | [82 HTTP operations](https://api.peec.ai/customer/v1/openapi/json) across 67 OpenAPI paths; aggregate reports, raw chats, citations, fan-out, shopping and agent traffic | API is Enterprise; MCP is on paid plans | API remains beta |
| 2 | [Scrunch](https://developers.scrunch.com/) | **92** | [44 operations](https://api.scrunchai.com/v1/openapi.json) across 31 OpenAPI paths; aggregate and raw responses, traffic, configuration, audits, signals and webhooks | Enterprise/custom | Strong surface, but a high access gate |
| 3 | [Rank Prompt](https://rankprompt.com/docs/v1/) | **90** | Brands, facts, async reports, raw responses, prompts, citations, competitors, audits, GA4/GSC, tasks and webhooks | API from Starter; separate API plans available | No independently captured operation total in this edition |
| 4 | [DataForSEO](https://docs.dataforseo.com/v3/ai_optimization-overview/) | **82** | Usage-priced LLM responses, ChatGPT UI scraping, mentions, historical metrics and top pages/domains | Public pay as you go | Builder-oriented; SOV and sentiment often need to be derived |
| 5 | [Keyword.com](https://keyword.com/docs/ai-visibility-api/) | **80** | 6 AI-visibility reads plus a separate SERP API; domains, terms, dashboard metrics, sentiment and citations | Included across self-serve plans and trial | Aggregate API; no raw answers or scan execution |
| 6 | [BeVisible](https://bevisible.app/docs/api) | **77** | 22 documented operations for visibility, crawler traffic, prompts, raw responses, citations, GSC and action briefs | API and MCP on Growth | Smaller, still-evolving surface |
| 7 | [Meltwater GenAI Lens](https://developer.meltwater.com/guides/ai-visibility/overview/) | **64** | Prompt/folder retrieval and analysis with visibility, sentiment and SOV metrics | Contract entitlement | Narrow interface; no raw-answer or scan workflow documented |

### API Score Breakdown

| Product | Docs /20 | Data /20 | Coverage /15 | Actions /15 | MCP /10 | Access /10 | Operations /10 | Total |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Peec AI | 20 | 20 | 15 | 13 | 10 | 7 | 9 | **94** |
| Scrunch | 20 | 20 | 15 | 15 | 9 | 4 | 9 | **92** |
| Rank Prompt | 17 | 18 | 13 | 15 | 9 | 9 | 9 | **90** |
| DataForSEO | 20 | 18 | 11 | 9 | 5 | 10 | 9 | **82** |
| Keyword.com | 19 | 13 | 13 | 7 | 10 | 10 | 8 | **80** |
| BeVisible | 16 | 17 | 12 | 11 | 4 | 9 | 8 | **77** |
| Meltwater GenAI Lens | 20 | 12 | 8 | 4 | 5 | 5 | 10 | **64** |

## Hosted MCP Leaderboard

Hosted MCP implementations are scored separately from APIs: normalized AI-search capability breadth (40), MCP interface quality (25), openness and developer experience (20), and trust, operations and result provenance (15).

The raw number of tools does not add points. Tool counts are easy to inflate with CRUD variants, aliases and generic administration tools.

| Rank | Product | Score | Tools | Read/write | Why it ranks here |
|---:|---|---:|---:|---|---|
| 1 | [Peec AI](https://docs.peec.ai/mcp/tools) | **95** | **76** | 33 read / 43 write | Broadest fully enumerated catalog, eight engine surfaces, field-level schemas, raw answers, shopping and agent traffic |
| 2 | [LLM Pulse](https://llmpulse.ai/features/mcp) | **93** | **48** | 40 read / 8 write | Strong GEO-native balance across metrics, raw evidence, AI traffic, recommendations and scoped actions |
| 3 | [Scrunch](https://developers.scrunch.com/mcp/tools) | **92** | **45** | Mixed | Deep reporting and response access plus configuration, statistically tested signals and agent-traffic import/export |
| 4 | [Profound](https://docs.tryprofound.com/mcp/overview) | **90** | **56** | 37 read / 19 state-changing | Deep enterprise surface spanning visibility, citations, sentiment, facts, shopping, bots, referrals, agents and projects |
| 5 | [OtterlyAI](https://docs.otterly.ai/mcp-server) | **86** | **32** | 24 read / 8 permission-gated write | Compact, unusually transparent catalog with OAuth and dynamic write registration |
| 6 | [MentionFlow](https://mentionflow.ai/docs/api/mcp) | **80** | **24** | 23 read / 1 metered write | Evidence-rich reads across visibility, answers, citations, sentiment, crawlers, traffic and content coverage |
| 7 | [Cituna](https://cituna.com/mcp) | **76** | **16** | 12 read / 4 write | Focused catalog with visibility, raw engine answers, audits, gaps, GSC and content-queue actions |
| 8 | [Keyword.com](https://keyword.com/docs/mcp/) | **74** | **67** | 20 writes in the full catalog | Excellent hybrid SEO MCP, but only six tools are specific to AI Visibility |
| 9 | [Scope](https://scope.online/agents) | **70** | **27** | 17 read / 10 action | Useful scans, citations, traffic and fixes, but current public pages disagree on tool and engine counts |

### MCP Score Breakdown

| Product | Capabilities /40 | Interface /25 | Openness /20 | Trust /15 | Total |
|---|---:|---:|---:|---:|---:|
| Peec AI | 38 | 25 | 18 | 14 | **95** |
| LLM Pulse | 40 | 24 | 17 | 12 | **93** |
| Scrunch | 38 | 24 | 16 | 14 | **92** |
| Profound | 40 | 24 | 12 | 14 | **90** |
| OtterlyAI | 35 | 24 | 17 | 10 | **86** |
| MentionFlow | 35 | 21 | 15 | 9 | **80** |
| Cituna | 30 | 23 | 14 | 9 | **76** |
| Keyword.com | 19 | 25 | 18 | 12 | **74** |
| Scope | 31 | 20 | 11 | 8 | **70** |

## MCP Tool-Count Leaderboard

This table answers the simple “how many tools?” question. It should not be read as a quality ranking.

| Rank | Product | Published or enumerated tools | Verification note |
|---:|---|---:|---|
| 1 | [Canonry](https://github.com/Canonry/canonry/blob/main/docs/mcp.md) | **206** | Public-source full catalog: 204 API tools plus two discovery tools; a small core loads first |
| 2 | [Peec AI](https://docs.peec.ai/mcp/tools) | **76** | Exact public catalog |
| 3 | [Keyword.com](https://keyword.com/docs/mcp/) | **67** | Exact public catalog; six AI-visibility-specific tools |
| 4 | [Cognizo](https://www.cognizo.ai/platform/mcp) | **62 claimed** | Tool names and schemas are not public; excluded from the scored leaderboard |
| 5 | [Profound](https://docs.tryprofound.com/mcp/overview) | **56** | Unique tools deduplicated from the current official reference |
| 6 | [LLM Pulse](https://llmpulse.ai/features/mcp) | **48** | Exact count of currently named tools; product copy rounds this to “more than 45” |
| 7 | [Scrunch](https://developers.scrunch.com/mcp/tools) | **45** | Exact public catalog |
| 8 | [OtterlyAI](https://docs.otterly.ai/mcp-server) | **32 possible** | Eight write tools appear only with write permission |
| 9 | [Scope](https://scope.online/agents) | **27 current** | Current enumeration; stale public copy also shows lower totals |
| 10 | [MentionFlow](https://mentionflow.ai/docs/api/mcp) | **24 current** | Current catalog; page heading still says 16 |
| 11 | [Rank Prompt](https://rankprompt.com/docs/v1/mcp/) | **20** | Hosted OAuth MCP |
| 12 | [Cituna](https://cituna.com/mcp) | **16** | Exact public catalog |
| 13 | [DataForSEO](https://github.com/dataforseo/mcp-server-typescript) | **4 generic** | Code-mode design: one generic API tool reaches the broader API surface |

## Capability Matrix

| Product | API | MCP | Raw answers | Citations | Sentiment | Competitors/SOV | AI traffic or crawlers | Writes/actions |
|---|---|---|---|---|---|---|---|---|
| Peec AI | Yes | Yes | Yes | Yes | Yes | Yes | Crawler/agent visits | Extensive configuration CRUD |
| Scrunch | Yes | Yes | Yes | Yes | Yes | Yes | Both | Prompts, brands, competitors, personas and traffic ingest |
| Rank Prompt | Yes | Yes | Yes | Yes | Yes | Yes | GA4/GSC | Scans, audits, tasks and webhooks |
| Profound | Yes | Yes | Yes | Yes | Yes | Yes | Both | Prompts, agents, projects, docs and knowledge bases |
| LLM Pulse | Yes | Yes | Yes | Yes | Yes | Yes | Both | Prompts, competitors, tags, content, recommendations and audits |
| OtterlyAI | Yes | Yes | Yes | Yes | Not evidenced in MCP catalog | Yes | Crawler/agent stats | Prompts, tags and audit creation |
| Keyword.com | Two REST APIs | Yes | No in AIV API | Yes | Yes | Yes | No | Broad SEO/project management; limited AIV actions |
| MentionFlow | Yes | Yes | Yes | Yes | Yes | Yes | Both | One metered fact-check action |
| Cituna | Yes | Yes | Yes | Yes | Not evidenced | Yes | GSC | Scans, gaps and content queue |
| Scope | No public REST reference found | Yes | Prompt results | Yes | Not evidenced | Yes | Both | Scans, tracking, competitors and fixes |

“Not evidenced” means that the capability was not found in the public interface reference used for this snapshot. It does not prove that the product lacks the feature in its dashboard.

## Category Leaders

- **Open/self-hosted:** [Canonry](https://github.com/Canonry/canonry) — source-visible, local SQLite, public OpenAPI and a progressive MCP catalog. It is separated from hosted SaaS scoring because users operate the service and supply provider keys themselves.
- **Hosted MCP breadth:** [Peec AI](https://docs.peec.ai/mcp/tools) — the strongest combination of a large catalog and unusually detailed public schemas.
- **GEO-native read/action balance:** [LLM Pulse](https://llmpulse.ai/features/mcp) — broad evidence retrieval plus a relatively small, scoped write surface.
- **Enterprise workflows:** [Profound](https://docs.tryprofound.com/mcp/overview) — analytics combined with agent, project, document and knowledge-base workflows.
- **Traditional SEO plus AI visibility:** [Keyword.com](https://keyword.com/docs/) — two REST APIs and one MCP spanning rank tracking and AI visibility.
- **Public pay-as-you-go data:** [DataForSEO](https://dataforseo.com/ai-optimization-api) — useful for teams building their own measurement product rather than buying a turnkey dashboard.
- **Self-serve scan automation:** [Rank Prompt](https://rankprompt.com/docs/v1/) — API access from Starter with async scans, raw responses, audits and webhooks.

## Watchlist and Exclusions

- **Cognizo** publishes a 62-tool total but not the tool names or schemas. It appears in the count table but cannot receive an interface score yet.
- **AI Sightline** has current public pages that disagree on whether its MCP exposes 26, 30, 30+ or 37 tools, and its developer page says the npm package is still on the roadmap. It can be added after the canonical catalog and installation path are reconciled.
- **Pendium** currently publishes conflicting totals for both its REST operations and MCP tools. It can be scored once one canonical reference is available.
- **BeVisible** has a useful documented API and says MCP is included on Growth, but no exact public MCP tool catalog was found.
- Products with only a homepage claim, a sales-gated deck or no canonical interface reference are not ranked.

## Methodology

### Eligibility

A product is ranked only when it exposes programmatic access directly related to AI-search visibility, citations, responses, referrals or the associated measurement workflow, and at least one core capability is supported by a live structured interface, official reference or public source repository. Evidence must be public without an NDA.

### Evidence Grades

- **A — Live verified:** a public endpoint returned valid structured metadata or an expected authentication/protocol response.
- **B — Structured:** an official OpenAPI document, MCP catalog or public implementation is available.
- **C — Reference:** official documentation enumerates the specific operations, parameters and results.
- **D — Marketing only:** an announcement or product claim without a reference. It receives no score.

All canonical MCP endpoints in the hosted shortlist returned an expected live protocol, method or authentication response on September 2, 2026. No authenticated customer data calls were made.

### MCP Scoring

Capability breadth is normalized into ten families: account/project configuration; prompts; runs and raw answers; visibility and position; citations and sources; competitors and SOV; sentiment and qualitative insight; history and segmentation; AI traffic/crawlers; and exports or downstream delivery. Aliases, bulk variants and CRUD splits do not create new capability points.

Interface quality covers discoverability, schemas, identifiers and descriptions, pagination/filtering/time ranges, authentication and reproducible protocol behavior. Openness covers public references, quickstarts, safe trial paths, SDKs/samples, access requirements, source availability and support. Trust covers security guidance, operational transparency, maintenance and result provenance.

### Counting Rules

- MCP tools are unique names in the documented or discoverable catalog for the stated tier and role.
- Resources and prompt templates are not counted as tools.
- Permission-gated tools are reported as “possible” when a vendor clearly documents dynamic registration.
- Full progressive catalogs are reported with their default-load behavior noted.
- API operations are distinct HTTP method and normalized-path pairs. Health, docs, login and billing routes are excluded where a machine-readable schema allows filtering.
- Raw operation and tool counts never break a score tie.

## Limitations and Corrections

- This is a programmatic-readiness benchmark, not a data-accuracy benchmark.
- Authenticated catalogs can vary by account, plan, role, permission, geography and feature flag.
- A large MCP may be a thin wrapper over an API; a small MCP may expose a few powerful aggregate tools.
- Public documentation can lag deployed software. Conflicts are penalized rather than silently resolved in the vendor's favor.
- Pricing, accuracy, coverage recall, latency and uptime require separate controlled tests.
- Vendor corrections are welcome through a pull request, but must include a public canonical source and an affiliation disclosure. Corrections update the evidence record; they do not purchase or guarantee placement.

## Primary Sources

- [Peec AI API](https://docs.peec.ai/api/introduction), [OpenAPI document](https://api.peec.ai/customer/v1/openapi/json) and [MCP tools](https://docs.peec.ai/mcp/tools)
- [Scrunch developer platform](https://developers.scrunch.com/), [OpenAPI document](https://api.scrunchai.com/v1/openapi.json) and [MCP tools](https://developers.scrunch.com/mcp/tools)
- [Rank Prompt API and MCP](https://rankprompt.com/docs/v1/)
- [DataForSEO AI Optimization API](https://docs.dataforseo.com/v3/ai_optimization-overview/) and [MCP source](https://github.com/dataforseo/mcp-server-typescript)
- [Keyword.com developer platform](https://keyword.com/docs/)
- [BeVisible API](https://bevisible.app/docs/api)
- [Meltwater GenAI Lens API](https://developer.meltwater.com/guides/ai-visibility/overview/)
- [Canonry API and MCP source](https://github.com/Canonry/canonry)
- [Profound API](https://docs.tryprofound.com/rest-api/introduction) and [MCP](https://docs.tryprofound.com/mcp/overview)
- [LLM Pulse API](https://llmpulse.ai/api-docs) and [MCP](https://llmpulse.ai/features/mcp)
- [OtterlyAI MCP](https://docs.otterly.ai/mcp-server)
- [MentionFlow MCP](https://mentionflow.ai/docs/api/mcp)
- [Cituna MCP](https://cituna.com/mcp)
- [Scope MCP](https://scope.online/agents)
