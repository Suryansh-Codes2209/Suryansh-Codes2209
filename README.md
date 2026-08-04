<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/hero-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/hero-light.svg">
  <img alt="Suryansh Chaudhary — Full-Stack AI Engineer, Bangalore. I ship LangGraph agents to production and open-source macOS tools." src="./assets/hero-dark.svg">
</picture>

<p align="center">
  <a href="https://suryansh.work"><b>Site</b></a> ·
  <a href="https://suryansh.work/blog"><b>Build logs</b></a> ·
  <a href="https://x.com/Suryansh_2001"><b>X</b></a> ·
  <a href="https://www.linkedin.com/in/suryansh-chaudhary-2209/"><b>LinkedIn</b></a> ·
  <a href="https://suryansh.work/suryansh.pdf"><b>Résumé</b></a>
</p>

---

## Now

- **MacGet 1.2** — YouTube & HLS downloads, browser-capture, signed auto-updates.
- **A multi-agent financial research desk** — LangGraph control plane, Vertex AI multimodal RAG data plane.
- **A build log every week** — the engineering, the trade-offs, and what broke.

---

## MacGet — native macOS download manager

<table>
<tr>
<td width="58%" valign="top">

<a href="https://github.com/Suryansh-Codes2209/Macget"><img src="https://img.shields.io/github/v/release/Suryansh-Codes2209/Macget?label=release&color=0a84ff&labelColor=161b22&style=flat-square" alt="Latest release"></a>
<a href="https://github.com/Suryansh-Codes2209/Macget/releases"><img src="https://img.shields.io/github/downloads/Suryansh-Codes2209/Macget/total?label=downloads&color=34c759&labelColor=161b22&style=flat-square" alt="Total downloads"></a>
<a href="https://github.com/Suryansh-Codes2209/Macget/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Suryansh-Codes2209/Macget?color=8e8e93&labelColor=161b22&style=flat-square" alt="License"></a>

<br>

Chunked HTTP parallelism that <b>adapts per host</b>, anti-leech CDN detection,
browser-extension capture over Native Messaging, and bundled <code>yt-dlp</code> for video.
Built in Swift on an actor-based concurrency engine — no polling, no shared mutable state.

<br>

<b>Free · Open source · macOS 26+</b>

</td>
<td width="42%" valign="top">

<img src="./assets/macget-demo.gif" alt="MacGet downloading a file with eight parallel chunks" width="100%">

</td>
</tr>
</table>

> [!TIP]
> **[Download MacGet →](https://github.com/Suryansh-Codes2209/Macget/releases/latest/download/Macget.dmg)** — or read [how the download engine works](https://suryansh.work/blog/building-macget-download-engine).

---

## How I build agents

The shape I reach for on every production agent — explicit state, small nodes, a hard grounding gate before anything reaches a user.

```mermaid
flowchart LR
    Q([Analyst question]) --> R{Router}
    R -->|filings| RAG[Vertex multimodal RAG]
    R -->|prices| MKT[Market data tools]
    RAG --> S[Synthesis node]
    MKT --> S
    S --> G{Grounding gate}
    G -->|fail| RAG
    G -->|pass| OUT([Analyst-grade report])

    style Q fill:#0a84ff22,stroke:#0a84ff
    style OUT fill:#34c75922,stroke:#34c759
    style G fill:#f0883e22,stroke:#f0883e
```

Written up in full: [architecting a financial AI analyst](https://suryansh.work/blog/how-we-architect-a-financial-ai-analyst-multi-agent) · [hard gates and soft gates](https://suryansh.work/blog/langgraph-prompt-injection-hard-soft-gates)

---

## Stack

**Daily:** `LangGraph` `LangChain` `Python` `FastAPI` `TypeScript` `React` `Swift` `Google Cloud Run`

<details>
<summary>Everything else I work in</summary>

<br>

| Area | Tools |
|---|---|
| **AI / Agents** | LangGraph · LangChain · Vertex AI RAG · Gemini & Claude APIs · eval + guardrail design |
| **Backend** | Python · FastAPI · Django · Node.js · PostgreSQL · Redis · MongoDB |
| **Frontend** | TypeScript · React · Next.js · Tailwind · Framer Motion |
| **Native** | Swift · SwiftUI · structured concurrency / actors |
| **Infra** | Google Cloud Run · Docker · GitHub Actions · CI/CD |

</details>

---

## Latest build logs

<!-- BLOG-POST-LIST:START -->- [MCP servers vs agent skills: the payload is the integration](https://suryansh.work/blog/mcp-servers-vs-agent-skills-tool-payload-design) — <sub>Aug 3, 2026</sub><br>- [MacGet 1.3.0: BitTorrent, book catalogs, and deleting my own adaptive concurrency](https://suryansh.work/blog/macget-1-3-0-bittorrent-book-catalogs-adaptive-concurrency) — <sub>Jul 30, 2026</sub><br>- [Automating blog cover art with Gemini 3 Pro Image: my &#39;no legible text&#39; rule was the bug](https://suryansh.work/blog/automating-blog-cover-art-gemini-3-pro-image) — <sub>Jul 26, 2026</sub><br>- [Claude Opus 5 vs Fable 5: how I&#39;m routing nodes in a LangGraph agent](https://suryansh.work/blog/claude-opus-5-vs-fable-5-routing-langgraph-agents) — <sub>Jul 26, 2026</sub><br><!-- BLOG-POST-LIST:END -->

<sub><a href="https://suryansh.work/blog">All posts →</a></sub>

---

## Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/2-most-commit-language.svg">
  <img src="./profile-summary-card-output/vue/2-most-commit-language.svg" alt="Most-used languages" width="49%">
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/3-stats.svg">
  <img src="./profile-summary-card-output/vue/3-stats.svg" alt="GitHub stats" width="49%">
</picture>

---

## Open to

- Collaborations on agent infrastructure and developer tooling
- Bug reports, feature ideas, and PRs on [MacGet](https://github.com/Suryansh-Codes2209/Macget)
- Talking shop about LangGraph, RAG evals, or Swift concurrency

**suryansh.codes2001@gmail.com**