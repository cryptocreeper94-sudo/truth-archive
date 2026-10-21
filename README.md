# TRUTH — Provenance-First Evidence Archive (public data)

> **Live:** [truth.tlid.io](https://truth.tlid.io)  
> **Author:** Andrews, Ronald Jason — DarkWave Studios LLC  
> **License:** CC-BY-4.0

---

## What this is

This repository is the **public evidence archive** behind [truth.tlid.io](https://truth.tlid.io): every claim card, every source record, every dig site, and the method that governs them. The site reads directly from this repository, so what you see here is exactly what the site shows.

It is a **case file system**, not a collection of beliefs. Right or wrong, everything is documented with its sources and confidence, and the reader decides. The method outranks any conclusion.

The git history is part of the record: every entry carries the time it was committed, and entries are demoted as well as promoted.

## The three iron rules

1. **Every claim carries a confidence tag.** DOCUMENTED / CONTESTED / SPECULATIVE. No untagged claims. Ever.
2. **Every link between claims is typed and tagged.** A connection is itself a claim. Speculative links never count as corroboration.
3. **Motive is argued last, from documented links only.** "Who benefits" is a conclusion the evidence earns, never an assumption the evidence is arranged around.

## Structure

```
README.md              - this file
METHOD.md              - the full specification: tiers, tags, link types, ID scheme
MANIFEST.md            - archive manifest
PHYSICAL_EVIDENCE.md   - physical evidence protocol
claims/                - claim cards: one file per claim, tagged and sourced
sources/tier-1/        - source records: physical survivors (manuscripts, maps,
                         statutes, patents, institutional records)
digs/                  - dig sites: investigation trenches gathering claims,
                         sources, and links around one question
links/                 - typed links between claims
evidence/              - physical evidence records (PE-YYYY-NNN)
verification/          - automated source and URL verification report
```

## How entries are added

New claims and sources are drafted by the Truth Sentinel research daemon under METHOD.md and committed here through the GitHub API. Commits from the daemon are prefixed `daemon:`. The daemon can never assign DOCUMENTED; every drafted claim starts at SPECULATIVE and must cite a Tier-1 source.

## Using the data

Every file is Markdown with YAML frontmatter, so it can be read with any Markdown or YAML tooling. To cite the archive, cite the specific file and commit, for example:

```
Truth Archive, claims/C-0086-<slug>.md, commit <sha>, https://github.com/cryptocreeper94-sudo/truth-archive
```

## What this archive is not

- Not a wiki of conclusions. Evidence and its sorting live here.
- Not a place where a pile of speculative links adds up to proof. It doesn't, and the tags exist so it can't.
- Not finished. The willingness to rule against ourselves is the feature.

---

## Ecosystem

| Node | URL |
|------|-----|
| Truth Archive | [truth.tlid.io](https://truth.tlid.io) |
| Observatory | [observatory.tlid.io](https://observatory.tlid.io) |
| DarkWave Studios | [darkwavestudios.io](https://darkwavestudios.io) |

© 2026 DarkWave Studios LLC
