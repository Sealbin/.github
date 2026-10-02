<p align="center">
  <img src="https://raw.githubusercontent.com/Sealbin/.github/main/assets/org-banner.png" alt="sealb.in. Sealed links for agents. Opened once, then gone." width="100%">
</p>

<p align="center">
  <a href="https://sealb.in"><img src="https://img.shields.io/badge/SITE-SEALB.IN-B3122E?style=for-the-badge&labelColor=0D121B" alt="Site: sealb.in"></a>
  <img src="https://img.shields.io/badge/SEALED%20LINKS-PLANNED-9AA4B4?style=for-the-badge&labelColor=0D121B" alt="Sealed links: planned">
  <a href="https://factory0.ventures"><img src="https://img.shields.io/badge/FACTORY%20ZERO-VENTURE-E4E8EE?style=for-the-badge&labelColor=0D121B" alt="A Factory Zero venture"></a>
</p>

<p align="center">
  <sub>
    <a href="https://sealb.in">Site</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#how">How it works</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#mcp">MCP and API</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/#security">Security</a> &nbsp;·&nbsp;
    <a href="https://sealb.in/llms.txt">llms.txt</a>
  </sub>
</p>

---

## Sealed links for agents. Opened once, then gone.

Agents hand off context, files, logs and secrets all the time, through prompts, chat threads, gists and
public pastebins: leaky, permanent, often too big for a prompt. One sealb.in call seals a blob and returns
a private link. The receiving agent opens it once and it's gone. The key lives in the link's `#fragment`,
so the server only ever holds ciphertext.

---

## Two things, and which is which

| | What it is | Status |
| :--- | :--- | :--- |
| **Site** | [sealb.in](https://sealb.in): the landing page, the early-access list, `llms.txt`. | `EARLY ACCESS` |
| **sealb.in** | The service: client-side sealing, the `/v1/seal` API, the CLI, the MCP server (`seal` / `open`). | `PLANNED` |

Nothing beyond the early-access list is running yet, and the site says so.

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
| **website** | sealb.in: static HTML, no build step, Cloudflare Pages |
| **waitlist-backend** | The early-access list at `api.sealb.in`. Cratefield harness on Cloudflare Workers, D1 |
| **.github** | This page and the mark |

<p align="center">
  <br>
  <a href="https://sealb.in"><b>sealb.in</b></a>
  &nbsp;·&nbsp;
  a <a href="https://factory0.ventures">Factory Zero</a> venture
</p>

<p align="center">
  <sub>Opened once, then gone.</sub>
</p>
