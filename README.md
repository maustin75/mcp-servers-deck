# MCP: Review and Opportunities

A self-contained, interactive presentation on **Model Context Protocol servers** —
what MCP is, how it compares to the alternatives, and where the opportunities are.
Written for an audience of portfolio architects.

**[`mcp-servers-deck.html`](mcp-servers-deck.html)** — one file, no build step, no
dependencies. Download it and open it in a browser.

Want it as a download? **[`mcp-servers-deck.html.zip`](mcp-servers-deck.html.zip)** is
the same deck, zipped. GitHub displays `.html` as source rather than rendering it, so
the zip is the quicker route to a copy you can actually open. The `.html` is the source
of truth — the zip is generated from it, so regenerate it after any edit:

```sh
zip mcp-servers-deck.html.zip mcp-servers-deck.html
```

## What's in it

Nineteen slides in six parts, about thirty minutes:

| Part | Slides | |
|---|---|---|
| **Why it matters** | 2 | the integration cost curve |
| **What it is** | 3–5 | host / client / server, one request end to end, the three primitives |
| **Where it fits** | 6–9 | vs. a REST API, vs. GraphQL, vs. A2A, and calling an agent |
| **How it works** | 10–12 | the stateless core, transports, a reference architecture |
| **Building it** | 13–15 | a working server, what not to build on, security |
| **The opportunity** | 16–19 | adoption, governance, what it could become, where to start |

Ten hand-drawn SVG diagrams, an animated request walkthrough with the real wire
frames on hover, a stateful/stateless before-and-after toggle, and presenter
notes on every slide.

## Using it

| Key | |
|---|---|
| `←` `→` `space` | move between slides |
| `P` | presentation mode — full screen, no chrome |
| `N` | presenter notes — full-height panel with pacing and *up next* |
| `B` | show / hide the contents sidebar |
| `O` | contents overlay |
| `F` | plain full screen |

Light and dark themes follow your system setting; the `◐` control overrides it.

## Accuracy

Every method name, field and code sample is taken from the
[**2026-07-28 specification**](https://modelcontextprotocol.io/specification/2026-07-28/changelog)
text rather than from memory or secondary write-ups. That revision made MCP a
stateless request/response protocol — if you have read older material, a fair
amount of it is out of date.

Where an adoption figure is disputed, the deck says so rather than quoting it.

Sources: [specification and changelog](https://modelcontextprotocol.io/specification/2026-07-28/changelog) ·
[release notes](https://blog.modelcontextprotocol.io/posts/2026-07-28/) ·
[Agentic AI Foundation](https://aaif.io/) ·
[Linux Foundation](https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation)

## Adapting it

The examples are deliberately generic (`incidents`, `crm`, `deploy`) — swap in
your own systems before presenting. The running order lives in one `ORDER` table
near the top of the inline `<script>`, so slides can be re-sequenced without
moving any markup. Slides marked `class="slide retired"` are kept in the file but
not shown; remove that one word to bring one back.
