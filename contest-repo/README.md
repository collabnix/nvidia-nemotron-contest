# 🚀 Nemotron 3 Super Build Contest

> **A 4-week build contest from Collabnix × NVIDIA. Ship something real with Nemotron 3 Super.**

🌐 **Portal:** [contest.collabnix.com](https://contest.collabnix.com)
💬 **Community:** [Collabnix Slack — #nemotron-contest](https://collabnix.com)
⭐ **Reference projects:** [awesome-nvidia-nemotron](https://github.com/collabnix/awesome-nvidia-nemotron)

---

## How it works

1. **Build something** with NVIDIA Nemotron 3 Super — agentic workflow, RAG app, fine-tune, deployment recipe, anything creative
2. **Push it to a public GitHub repo** with a clear README and a demo
3. **Submit here** by [opening a Submission issue](../../issues/new?template=submission.yml) — your project goes live on the [public wall](https://contest.collabnix.com#wall) instantly
4. **Wait for judging** at the end of the contest window. Winners announced shortly after.

That's it. No registration form, no waitlist, no gated forum.

## Tracks

| # | Track | What fits here |
|---|---|---|
| 1 | Agentic Workflows | Multi-agent systems, tool-using agents, MCP integrations |
| 2 | RAG & Long Context | Retrieval, document/codebase chat, long-window applications |
| 3 | Fine-tuning & Distillation | Domain/language adaptation, LoRA, SFT, evals |
| 4 | Deployment & Infra | TensorRT, vLLM, Triton, Docker, Kubernetes recipes |
| 5 | Wild Card | Creative apps, games, voice, vision, education — surprise us |

Pick **one** track per submission.

## Judging criteria

Each submission scored on four dimensions, weighted equally:

- **Technical execution** — does it work, is the code good, are the trade-offs sound
- **Originality** — is this a novel idea or a fresh angle on an existing one
- **Real-world utility** — could someone actually use this
- **Documentation quality** — README, demo, write-up — can a stranger pick it up

## Judges

- **Megh Makwana** — NVIDIA, AI Solutions
- **Utkarsh Uppal** — NVIDIA, Solution Architect
- **Savitha Pareek** — NVIDIA, Senior HPC & AI Architect
- **Ajeet Singh Raina** — Docker, Founder of Collabnix

## Prizes

🥇 **Grand Prize** — Cash + NVIDIA hardware + featured on NVIDIA Developer blog + speaker slot at next Collabnix meetup
🥈 **Runner-up** — Cash + NVIDIA swag + Collabnix feature
🏆 **Track Winners** — Recognition per track + swag + permanent feature in Awesome-Nemotron

## Submission rules

- **Open source license required** (MIT, Apache 2.0, BSD, GPL — your choice)
- **Public GitHub repo only** — no gists, no private repos
- **Built during the contest period** — substantial work after Week 0. Recycled projects with cosmetic changes will not be accepted
- **You retain ownership** — Collabnix and NVIDIA may feature your work (with credit) but IP stays with you
- **One submission per team** — teams of 1–4 people
- **Nemotron must be used meaningfully** — not as a token mention. Judges will look closely at this.

Read the full FAQ on the [contest portal](https://contest.collabnix.com#faq).

## Get help

- **Stuck on setup?** Slack #nemotron-contest channel — fastest replies
- **Question about rules?** [Open a question issue](../../issues/new?template=question.yml)
- **Office hours:** Every Friday 6 PM IST during the contest window — link in Slack

---

## For maintainers

This repo is the submission backend for the contest portal. Submissions arrive as GitHub Issues (label: `submission`) and the portal at [contest.collabnix.com](https://contest.collabnix.com) fetches them via the GitHub API and renders them as a live wall.

**Repository structure:**
```
.github/
  ISSUE_TEMPLATE/
    submission.yml    # Main contest submission form
    question.yml      # Questions / help requests
    config.yml        # Disables blank issues, adds Slack link
  workflows/
    process-submission.yml   # Auto-labels, validates, welcomes submitters
README.md             # This file
```

**Labels used:**
- `submission` — auto-applied to every entry
- `track-1` through `track-5` — auto-applied based on selected track
- `needs-review` — default state for unjudged submissions
- `needs-fix` — auto-applied when repo URL is invalid; removed when fixed
- `shortlisted` — applied by judges
- `winner` — applied by judges after results

**Manual judge actions:**
- Comment with feedback on submissions
- Apply `shortlisted` label after first review pass
- Apply `winner` label and pin issue after results announced

---

*Built with ☕ in Bengaluru by [Collabnix](https://collabnix.com).*
