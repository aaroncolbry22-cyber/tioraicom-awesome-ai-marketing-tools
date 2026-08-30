# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 291 |
| Shortlisted after scope filtering | 135 |
| **Published** | **97** |

## Why candidates were dropped

- **Marketing is possible, not primary.** The largest exclusion by a wide margin. A general assistant that can produce a subject line is not an email marketing tool.
- **Belongs in the search repository.** Keyword, SERP, technical SEO, and AI-visibility tools were moved to `awesome-ai-seo-tools` rather than listed twice.
- **Generic writing tool.** Excluded unless it carries campaign, channel, brand-voice, or audience context. Writing well is not marketing.
- **Agency dressed as software.** Several entries turned out to be a service with a dashboard attached.
- **Enterprise suite with no separable product.** A marketing cloud is a procurement decision, not a tool a reader can try, and is listed only where the AI capability is a distinct product.
- **Category already well covered.** Applied hardest to content generation, where the count could have doubled without helping anyone choose.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 97 distinct external URLs were checked:
89 answered normally, 8 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
