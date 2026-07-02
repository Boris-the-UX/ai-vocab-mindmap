# Product

## Register

product

## Users

UX researchers on the team (including the author) who need a shared vocabulary for AI/LLM concepts as they apply to UX research work. The primary mode of use is a **learning path**: someone works through a branch of the mind-map top to bottom to build real understanding of a cluster of related terms, rather than a one-off dictionary lookup. Search still exists as a secondary utility for jumping straight to a known term, but it is not the primary interaction the design should optimize for.

## Product Purpose

A single-page reference tool that turns a flat glossary of AI/UX-research terms into a navigable mind-map: pick a branch (cluster of related concepts), read terms in that branch as cards, then open a term to see its full definition, why it matters for UX research specifically, and its related concepts. Success looks like a teammate finishing a branch with a working mental model of that cluster, not just having skimmed definitions.

## Brand Personality

Warm and approachable — the opposite of a clinical technical reference. This is a teaching tool for newcomers on the team as much as a lookup tool for experienced researchers, so it should feel encouraging and inviting rather than dense or intimidating. Soft edges, a guiding hand through the material, tone that assumes the reader is learning rather than already an expert.

## Anti-references

Avoid the generic "AI SaaS" visual scaffolding: gradient text, cream/sand near-white backgrounds, uniform card grids as the default answer for every layout problem, tiny uppercase tracked eyebrows, numbered section markers as decoration. The current build already leans into indigo/slate + card grids in a fairly generic way — that's a starting point to move past, not a constraint to preserve.

## Design Principles

- **Guide, don't just list.** The branch-first navigation should read as a guided path through a topic, not a flat filterable table; sequence and grouping carry teaching intent.
- **Warmth over sterility.** Every surface should feel like it was written by someone who wants the reader to succeed, not like an API reference.
- **Definition + application, always paired.** Every term shows both what it means and why a UX researcher specifically should care — never one without the other.
- **Built for a team, not just one person.** Copy and structure should hold up for a newcomer seeing a term for the first time, not just the original author.
- **Earn every visual cliché before using it.** No gradient text, no cream backgrounds, no reflexive card grid — if a pattern from the anti-references shows up, it must be deliberately justified.

## Accessibility & Inclusion

Standard best practice: solid color contrast (body text ≥4.5:1), full keyboard navigation (branch nav, search, term cards, related-term chips, detail panel), and `prefers-reduced-motion` support for any added motion. No additional stated requirements beyond that baseline.
