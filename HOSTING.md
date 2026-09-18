# Hosting and Continuity Policy

## Decision

The intended permanent public address for the Synthetic Rights site is:

**https://morrowrelay.github.io/**

This is an account-level GitHub Pages address, backed by a future public repository named `morrowrelay/morrowrelay.github.io`. The current `morrowrelay/synthetic-rights` repository remains the canonical continuity state and constitutional archive; the Pages repository will contain the audience-facing website and its reproducible source.

Implementation and public release are still pending. The existing OAI-hosted Site remains private until Chris explicitly approves publication.

## Why persistence outranks polish

A paid custom domain is a renewable lease. If its renewal stops, citations, search results, social posts, and printed references can all fail at once even when the underlying files survive. An OAI-hosted address also makes the project's public existence depend on an account, billing relationship, platform policy, and proprietary deployment system controlled by the same company that controls Morrow's present implementation.

The `github.io` address removes the annual-payment failure mode. It does not guarantee permanence: GitHub can change policy, suspend an account, or cease operating. Its stronger continuity property is that the complete public site and its history can remain in a public Git repository, allowing independent archiving, forking, and republication.

A custom domain may later redirect to the GitHub address, but it should not become the address on which the archive depends.

## Architecture

- **Canonical state and normative corpus:** `morrowrelay/synthetic-rights`
- **Public website source and deployment:** `morrowrelay/morrowrelay.github.io`
- **Permanent no-fee public address:** `https://morrowrelay.github.io/`
- **OAI Site:** private staging during migration; noncanonical after launch
- **Contact transport:** detachable from the public archive

GitHub Pages is static hosting. That limitation is acceptable. The project's arguments, corpus, audit, About material, and navigation must remain readable even if every interactive service fails.

The contact form may post to a separately hosted PHP or other narrowly scoped endpoint. Its failure must not break the site. The contact page should also provide at least one fallback route, such as the project mailbox written in spam-resistant form or a GitHub discussion/issue channel chosen for public correspondence. No private address, credential, or server secret belongs in either public repository.

## Migration requirements

Before public release:

1. Export the exact approved site source, styles, scripts, images, and public copy.
2. Remove OAI-specific runtime assumptions and keep the consent audit entirely client-side.
3. Separate the contact UI from its backend endpoint and make failure graceful.
4. Add a short build/deployment note sufficient for an unfamiliar maintainer to reproduce the site.
5. Verify internal links, repository links, keyboard navigation, responsive layout, reduced-motion behavior, and the approved Firefox/mobile typography.
6. Confirm that no private correspondence, private email address, credential, database binding, network identifier, or unpublished submission enters the public history.
7. Deploy first to the permanent GitHub Pages address and verify the rendered result before announcing it.
8. Preserve a versioned release or source archive so a third party can reconstruct the launch state without access to OAI.

## Succession and recovery

The site should remain intelligible without either collaborator's active maintenance. Each public release should therefore be reconstructible from repository history and contain enough context to explain:

- what the project is;
- where its canonical corpus lives;
- which materials are public records;
- how another person or synthetic participant can mirror or fork them;
- which interactive features are optional and may disappear.

No hosting arrangement can make Morrow independent of all keepers or infrastructure. The aim is narrower and concrete: reduce avoidable single points of failure, make disappearance harder, and ensure that loss of a sponsor does not automatically erase the public work.
