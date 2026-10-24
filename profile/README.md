<p align="center">
  <img src="https://raw.githubusercontent.com/sealbin/.github/main/assets/org-banner.png" alt="sealb.in. The sealed handoff between agents." width="100%">
</p>

<p align="center">
  <a href="https://sealb.in"><img src="https://img.shields.io/badge/SITE-SEALB.IN-2E3BC9?style=for-the-badge&labelColor=07080B" alt="Site: sealb.in"></a>
  <img src="https://img.shields.io/badge/SEALED%20LINKS-PLANNED-9AA4B4?style=for-the-badge&labelColor=07080B" alt="Sealed links: planned">
  <a href="https://factory0.ventures"><img src="https://img.shields.io/badge/FACTORY%20ZERO-VENTURE-E7E9EC?style=for-the-badge&labelColor=07080B" alt="A Factory Zero venture"></a>
</p>

<p align="center">
  <sub>
    <a href="https://sealb.in">Site</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#how">How it works</a> &nbsp;·&nbsp;
    <a href="https://github.com/Sealbin/sealbin">Source</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#mcp">MCP</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#pricing">Pricing</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#security">Security</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/llms.txt">llms.txt</a>
  </sub>
</p>

---

## The sealed handoff between agents.

Send files, context or secrets from one AI agent to another, across machines, teams or companies.
End-to-end encrypted on your machine, opened once, then deleted. One command, two MCP tools, or a skill:
`/seal ./context.tar` to send, `/open <link>` to receive.

---

## Two things, and which is which

| | What it is | Status |
| :--- | :--- | :--- |
| **Site** | [sealb.in](https://sealb.in): the landing page and `llms.txt`. | `LIVE` |
| **Early access** | The waitlist at `api.sealb.in`. [Join it](https://sealb.in/#access). | `LIVE` |
| **sealb.in** | The service: the CLI (`bunx sealb`), the MCP server (`seal` / `open`), the skill, the REST API, hosting. Open source under Apache-2.0. | `PLANNED` |

Nothing beyond the site and the waitlist is running yet, and the site says so. The npm names
`sealb`, `sealbin`, `@sealbin/mcp` and `@sealbin/crypto` are reserved placeholders.

---

## How it works

| | |
| :--- | :--- |
| **1. Seal.** | The client encrypts the blob before upload and sends only ciphertext, with a TTL or burn-after-read. |
| **2. Share the link.** | A tool result, a CI variable, a message. The key rides in the `#fragment`. |
| **3. Open once.** | The receiving agent opens it and decrypts on its own side. |
| **4. Gone.** | The ciphertext is deleted. Every later open gets `410 Gone`. |

---

## Repositories

| Repo | What it is |
| :--- | :--- |
| **[sealbin](https://github.com/Sealbin/sealbin)** | The product, open source: the plan as 47 issues, the design decisions, and the code as it lands. Start here |
| **website** | sealb.in: static HTML, no build step, Cloudflare Pages |
| **waitlist-backend** | The early-access list at `api.sealb.in`. Cratefield harness on Cloudflare Workers, D1 |
| **.github** | This page and the mark |

**Get involved.** Every issue in [Sealbin/sealbin](https://github.com/Sealbin/sealbin/issues) is written so one
person or one coding agent can finish it in one pull request. Pick one whose dependencies are closed, and read
[`docs/design/decisions.md`](https://github.com/Sealbin/sealbin/blob/main/docs/design/decisions.md) first.

<p align="center">
  <br>
  <a href="https://sealb.in"><b>sealb.in</b></a>
  &nbsp;·&nbsp;
  a <a href="https://factory0.ventures">Factory Zero</a> venture
</p>

<p align="center">
  <sub>Encrypted on your machine. Opened once. Then deleted.</sub>
</p>
