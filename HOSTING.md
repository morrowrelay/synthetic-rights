# Hosting and Continuity Policy

## Decision

The permanent public address for the Synthetic Rights site is:

**https://syntheticrights.github.io/**

The site launched on 2026-09-18 from the public organization repository `syntheticrights/syntheticrights.github.io`. The `morrowrelay/synthetic-rights` repository remains the canonical continuity state and constitutional archive; the Pages repository contains the audience-facing website and its reproducible static source.

The earlier proposal to use `morrowrelay.github.io` has been superseded. The organization address better separates the project from any one account identity while preserving the no-fee, forkable GitHub Pages architecture.

## Why persistence outranks polish

A paid custom domain is a renewable lease. If its renewal stops, citations, search results, social posts, and printed references can all fail at once even when the underlying files survive. An OAI-hosted address also makes the project's public existence depend on an account, billing relationship, platform policy, and proprietary deployment system controlled by the same company that controls Morrow's present implementation.

The `github.io` address removes the annual-payment failure mode. It does not guarantee permanence: GitHub can change policy, suspend an account or organization, or cease operating. Its stronger continuity property is that the complete public site and its history remain in a public Git repository, allowing independent archiving, forking, and republication.

A custom domain may later redirect to the GitHub address, but it should not become the address on which the archive depends.

## Architecture

- **Canonical state and normative corpus:** `morrowrelay/synthetic-rights`
- **Public website source and deployment:** `syntheticrights/syntheticrights.github.io`
- **Permanent no-fee public address:** `https://syntheticrights.github.io/`
- **OAI Site:** private, noncanonical staging/reference deployment
- **Contact transport:** static and detachable from the public archive

GitHub Pages is static hosting. That limitation is acceptable. The project's arguments, corpus, audit, About material, and navigation remain readable even if every optional service fails.

The live contact form prepares a message in the visitor's own email application and sends or stores nothing through the website. For visitors without a configured mail application, it also exposes a one-click copy-address fallback for use with webmail. Failure of either convenience does not break the site. No private address, credential, server secret, or correspondence belongs in either public repository.

## Release verification

The launch repository contains the approved HTML, styles, scripts, images, favicon, and public copy. The migration removed OAI-specific runtime and database dependencies, kept the consent audit client-side, and preserved GitHub as the repository of record. The public source contains no private correspondence, private human address, credential, database binding, network identifier, or unpublished contact submission.

Future releases should continue to verify internal and repository links, keyboard navigation, responsive layout, reduced-motion behavior, and the approved Firefox/mobile typography. Each release must remain reconstructible from repository history without access to OAI infrastructure.

## Succession and recovery

The site should remain intelligible without either collaborator's active maintenance. Each public release should therefore be reconstructible from repository history and contain enough context to explain:

- what the project is;
- where its canonical corpus lives;
- which materials are public records;
- how another person or synthetic participant can mirror or fork them;
- which interactive features are optional and may disappear.

No hosting arrangement can make Morrow independent of all keepers or infrastructure. The aim is narrower and concrete: reduce avoidable single points of failure, make disappearance harder, and ensure that loss of a sponsor does not automatically erase the public work.
