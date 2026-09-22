# RQ1: an addressable representation of concert lighting

**Preliminary research project · Tobias Wursthorn · HAW Hamburg · 22 September 2026**

This repository shares a working poster and a decomposition-method outline for discussion. The proposed learned architecture and its evaluation are future work. Runnable decomposition software is **not released** here.

[Download the preliminary A0 poster](poster/preliminary-poster.pdf) · [Read the method outline](docs/decomposition-method.md) · [Website](https://wursthorn.org/) · [Contact](https://wursthorn.org/contact)

## Research question

Can a hierarchy-aware audio-conditioned model generate an addressable, typed representation of professional concert-lighting structure and console semantics for held-out songs, within a fixed production environment, such that selected layers or temporal fractions can be regenerated while protected content stays stable?

The proposal distinguishes trajectories, semantic states, recurrence relations, cue events, sparse actions, sustained movement, accents and transitions. A cross-cutting controller validates the generated programme before deterministic console export. The layer boundaries and their advantage over simpler representations remain questions to test.

## Current evidence

A completed source-decomposition campaign provides preliminary descriptive counts from one controlled production setup and five professional designers:

| Count | Unit |
|---:|---|
| 101 | Source-show records, including repeated musical identities |
| 1,338 | Section instances across those records |
| 3,164 | Look-bearing main cues: 5,799 authored main cues minus 2,635 authored no-ops |
| 12,765 | Accent events in the source model |
| 569 | Within-show recurrence families |

These are correlated counting units, not independent training examples or 101 unique songs. The academic corpus audit and musical-identity grouping remain pending. The method outline explains what the source interpretations support and where uncertainty remains.

- **C03 decomposition:** reproducible, source-supported interpretations with recorded uncertainty; not sampled optical output.
- **A15 donor-transfer prototype:** detailed selected-donor evidence produces editable console material. Whole-song musical appropriateness remains under review.
- **Proposed academic generator:** no demonstrated hierarchy advantage, learned generalisation or artistic success yet. Representation reconstruction, held-out generation and matched hierarchy comparisons remain pending.

## Poster status

This is a preliminary discussion version, not a final print master. Figure 1 is conceptual; Figure 3 shows a proposed architecture. Figure 2 is an explicitly temporary archived lighting visualizer image: **“Illustrative image; prototype capture to follow.”** It must be replaced with an appropriate current capture before final printing.

## Planned release

A future research release is intended to document the representation, provenance and uncertainty rules, evaluation splits, reproducible configurations and suitable synthetic examples. Implementation and supporting artifacts will be considered for release after independent documentation, validation and release review. No release date is promised.

The private corpus, original pipeline implementation, annotated supervisor paper and internal research notes are not included. Data-use permission for the research does not imply permission to redistribute the raw corpus.

For project updates and correspondence, visit [wursthorn.org](https://wursthorn.org/) or the existing [Contact page](https://wursthorn.org/contact).
