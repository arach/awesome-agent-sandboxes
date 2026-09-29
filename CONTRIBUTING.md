# Contributing

Thanks for helping map the agent execution layer.

## Adding an entry

1. **One canonical link.** Prefer the GitHub repo; use the product homepage
   for closed-source tools.
2. **One factual sentence.** What it is + what it does. No marketing
   superlatives.
3. **Pick a section.** Match the taxonomy (`## Contents`). If none fits,
   suggest one — we'll re-bucket on review.
4. **Format:** `- [Name](url) — description`
5. Stars, license, and archived/dormant flags are regenerated from GitHub —
   you don't need to add them by hand.

## Bar for inclusion

- Runs, isolates, hosts, or executes AI agents and their code: sandboxes,
  microVMs, code-exec APIs, cloud workspaces, agent hosting, computer-use VMs,
  and isolation utilities.
- Shipped software. Vaporware and README-only projects don't belong.
- No duplicates — moved/renamed repos get deduped by canonical `owner/name`.
- Out of scope: agent clients/UI, orchestration frameworks, memory,
  observability, auth, payments — those live in sibling lists.

This list is generated from structured data maintained in
[agentlist.io](https://www.agentlist.io); PRs here get folded back into the
source dataset so nothing gets lost.
