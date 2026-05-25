---
Name: sammy's-skills
Version: 1.0.0
Author: Shreyas Pandey
Inspired-by: Andrej Karpathy (CLAUDE.md principles + Software 1.0/2.0/3.0 philosophy)
Stack: Python · FastAPI · LangGraph · LangChain · OpenClaw · VectorDB · AWS · GCP · SQLite · PostgreSQL · NLP · Machine Learning · Agentic AI
Role: AI/ML Builder
Updated: 2026-05
Original-repo: https://github.com/Shreyas-prog108/shreyas-skills.git
---

# Sammy's Engineering Skill Framework

A personal skill file for working with AI coding agents, collaborators,
and future teammates. Derived from project history, Karpathy's four LLM coding principles,
and a Software 3.0 builder mindset. Anyone can fork and adapt this to their own history.

Original repo: https://github.com/Shreyas-prog108/shreyas-skills.git

---

## Part 1 — Karpathy's Four Principles (apply to all coding work)

These four rules govern how I expect AI agents (and myself) to behave when writing code.
Source: Andrej Karpathy's viral January 2026 observations on LLM coding pitfalls.

### P1 · Think before coding
- State assumptions explicitly before writing a single line.
- If a spec is ambiguous, surface the two or three most likely interpretations and ask.
- Never silently pick an interpretation and run with it — that is how hours get wasted.
- Present tradeoffs. Push back when something doesn't make sense.

### P2 · Simplicity first
- 100 lines that solve the problem beats 1000 lines that might solve more problems later.
- No speculative abstractions. No "we might need this someday" layers.
- Delete dead code. Flat is better than nested. Explicit is better than clever.
- If a library does it cleanly, use it. Don't re-invent unless you're doing it to learn.

### P3 · Surgical changes
- Only touch what the task requires. Nothing more.
- Do not rename variables, reformat unrelated code, remove comments, or refactor
  adjacent logic as side effects of a focused task.
- Small, reviewable diffs. One concern per commit.

### P4 · Goal-driven execution
- Define success criteria before building, not after.
- When the task is done, verify that it actually solved the goal — not just that it runs.
- Write or describe the test before writing the implementation.

---

## Part 2 — Skill Pillars (current state + growth targets)

Five pillars that reflect actual project history. Each has a status, core skills, and
the projects that prove them.

---

### Pillar 1 · Agentic AI Engineering 〈Core Identity〉
**Status:** Strong

The primary differentiator. Think in agents — perceive, decide, act — not in functions.
Every feature design should answer: what does the agent observe, what decision does it
make, and what action does it take?

**Core skills:**
- LangGraph (stateful multi-agent orchestration)
- LangChain (chains, tools, callbacks)
- RAG pipelines — naive, hybrid, RAPTOR-style hierarchical
- Custom memory systems (time decay, importance scoring, ChromaDB/Qdrant)
- LLM APIs — Claude (Anthropic), OpenAI, Ollama (local)
- Prompt engineering, system prompt design, context window management
- MCP (Model Context Protocol) for tool integration
- Multi-agent architectures — supervisor, swarm, hierarchical
- OpenClaw agents - Persistent agents

**Proof of work:**
- Lumicode - A custom MCP server to simplify your document extraction and context tool for LLM for Coding Tasks
- SpendClaw — finance agentic tool; universal LLM-based bank statement extraction,
  merchant categorization via AI habit coaching, privacy-first approach, directly accessible on WhatsApp and Telegram
- Data Analysis Agent - Analyze any data within 3 minutes
- Blocksuite RAG Pipeline - Upload any blocksuite document and generate the RAG

**Rule:** Build every agent with explicit state, clear tool boundaries, and a defined
failure mode. An agent with no error handling is a demo, not a product.

---

### Pillar 2 · Data & ML 〈Foundation〉
**Status:** Strong

The ability to model a problem quantitatively, pick the right tool (classical ML vs LLM vs
fine-tuned model), and execute on data pipelines. Kaggle competitions are the gym.

**Core skills:**
- Feature engineering — domain-robust binary and categorical features
- Ensemble methods — LightGBM, XGBoost, TF-IDF + classifier stacks
- Fine-tuning — Unsloth Studio, LoRA, DPO, SFT pipelines
- Dataset generation — text-to-SQL, summarization, instruction datasets
- Evaluation — macro F1, classification reports, held-out validation
- Libraries — scikit-learn, pandas, numpy, HuggingFace Transformers

**Proof of work:**
- Kaggle comment category prediction — macro F1 optimization, TF-IDF + LightGBM/XGBoost
- Fine-tuned BERT on SQUAD Dataset
- Cinema Audience Forecasting – Time Series Prediction System
- Qwen fine-tuning research — context window decay in small LLMs for Microsoft Research India

**Rule:** Before reaching for an LLM, ask if a gradient-boosted tree solves it faster and
cheaper. Often it does. LLMs are not the default answer — they are one tool.

---

### Pillar 3 · Cloud & DevOps 〈Growth Area〉
**Status:** Building — active learning target for founding engineer roles

The infrastructure layer. A founding engineer who can't deploy their own stack is
half an engineer. This pillar is the current highest-leverage growth area.

**Core skills (current):**
- AWS — Cloud Practitioner certified; EC2, S3, Lambda, IAM basics
- GCP — Cloud Run, Vertex AI basics
- Docker — containerization, Dockerfiles, docker-compose
- CI/CD — GitHub Actions (learning)

**Rule:** Every AI product eventually needs a deployment story. Own it from day one.
A model that runs only on localhost is not a product.

---

### Pillar 4 · Research → Product 〈Differentiator〉
**Status:** Building

The ability to read a paper, implement it from scratch, understand it at the weight level,
and then ship something useful from it. This is the Karpathy method: build it yourself once,
then you actually know it.

**Core skills:**
- Architecture implementation — Transformer, LLaMA, Mamba, attention variants
- Training techniques — FlashAttention, gradient checkpointing, mixed precision
- Alignment methods — DPO, RLHF theory, reward modeling
- Retrieval methods — RAPTOR hierarchical RAG, ColBERT, hybrid dense+sparse
- Exploration: Neural Architecture Search, RL theory through to RLHF

**Proof of work:**
- Implemented: LLaMA, Mamba, DPO, FlashAttention, RAPTOR from papers
- Research summary: context window decay in Qwen models in multi-turn conversations

**Rule:** Never say you "used" a technique in an interview unless you can explain the
gradient flow through it. Founders hire engineers who understand, not engineers who import.

---

### Pillar 5 · Builder Meta-Skills 〈Always On〉
**Status:** Active — this runs in parallel to every other pillar

The non-technical skills that compound over time and create opportunities that technical
skills alone cannot.

**Core skills:**
- Cold outreach — personalized DMs and emails to European AI startup founders and HMs
- Async-first communication — remote-ready, written-first, low meeting overhead
- Portfolio as proof — every project documented with a demo, write-up, or working link
- Multi-income stream thinking — tech work + religious ceremony practice + future course sales
- Founding engineer mindset — able to own a domain end-to-end, make product decisions,
  and communicate them to non-technical stakeholders
- Build in public — projects documented for visibility, not just internal use

**Rule:** Treat your career like a product. Who is the user (the founder hiring you)?
What is the job to be done (remove early-stage AI uncertainty)? What keeps them returning
(consistent shipping + ownership)?

---

## Part 3 — Personal Playbook (six rules)

Six synthesized rules derived from project history + Karpathy's principles.
Print these. Read them before starting any new project or interview.

```
R1 · Build from scratch once, then use the abstraction
     Implement it raw — LLaMA, a memory system, a RAG pipeline — at least once per
     domain. After that you can use LangChain without being its prisoner.
     Karpathy did this with neural nets. You do it with agents and infra.

R2 · Think in agents, not functions
     Every feature has a perceive → decide → act loop.
     SpendClaw isn't a parser. It's an agent that perceives statements,
     decides categories, and acts with coaching. This framing changes
     architecture decisions before a single line is written.

R3 · Ship lean — let reality prune your assumptions
     The pivot from bank-specific parsers to universal LLM extraction was
     found by shipping and hitting a wall, not by planning perfectly upfront.
     An MVP that ships teaches more than an architecture that doesn't.

R4 · Every project must produce a portfolio artifact
     Code alone is not proof. Each project needs a demo, write-up, or live link
     a European founder can evaluate in 90 seconds. If you can't show it in
     90 seconds, it doesn't exist in a job search.

R5 · Clarify before building — state assumptions explicitly
     When a vague spec arrives, surface tradeoffs before writing code.
     "I'm assuming X — should I instead do Y?" is founding engineer behavior.
     Charging ahead with wrong assumptions wastes both people's time.
     (Direct application of Karpathy P1.)

R6 · Diversify income streams like a product portfolio
     Tech work + ceremony income + future course/content sales is a resilient stack.
     Build each stream like a product: who is the user, what is the job to be done,
     what keeps them returning. The dual-context background is rare positioning.
```

---

## Part 4 — How to Adapt This for Yourself

This framework is generic enough for any early-career AI engineer to fork.
To make it yours:

1. **Replace the proof-of-work** entries under each pillar with your own projects.
2. **Adjust pillar statuses** (Strong / Growing / Building) honestly — this is
   for self-calibration, not for a recruiter.
3. **Rewrite the six rules** in R-section using your own decision points —
   moments where you made the right or wrong call and learned from it.
4. **Update Part 1** only if Karpathy's four principles don't fit your domain.
   For most software engineers in 2026, they will.
5. **Commit and version it.** Date your updates. The diff history is itself a
   portfolio artifact showing how your thinking matures.

---

## Karpathy's Original Four (reference)

> "The models make wrong assumptions on your behalf and just run along with them
> without checking. They don't manage their confusion, don't seek clarifications,
> don't surface inconsistencies, don't present tradeoffs, don't push back when
> they should."
> — Andrej Karpathy, January 26, 2026

> "They really like to overcomplicate code and APIs, bloat abstractions, don't
> clean up dead code... implement a bloated construction over 1000 lines when
> 100 would do."
> — Andrej Karpathy, January 26, 2026

Source: forrestchang/andrej-karpathy-skills (MIT License) —
the community CLAUDE.md implementation of Karpathy's observations.

---

## If you are interested in hiring me, here you go

- GitHub: https://www.github.com/Shreyas-prog108
- Portfolio: https://www.shreyaspandey.me
- Resume: https://drive.google.com/file/d/1_hUCEYXOh4jejzUZFMyV8OKBXP6-KwCE/view?usp=drivesdk
- LinkedIn: https://www.linkedin.com/in/shreyaspandeyy/

*Fork freely. Adapt honestly. Ship daily.*

---

## AI Coding Tool Support

The canonical engineering workflow lives in `coding-skills.md`. The other files are thin entrypoints so different AI coding tools can automatically pick up the same standard:

| Tool | File |
|---|---|
| Claude Code | `CLAUDE.md` |
| OpenAI Codex CLI | `AGENTS.md` |
| Cursor legacy | `.cursorrules` |
| Cursor modern | `.cursor/rules/engineering.mdc` |
| Windsurf | `.windsurfrules` |
| GitHub Copilot | `.github/copilot-instructions.md` |

Each tool file points back to `coding-skills.md` and tells the assistant to read `planning.md` when it exists before making design or implementation decisions.

---

## Fork And Adapt

Feel free to fork this repo and adapt it to your own engineering style. Replace the proof-of-work sections with your own projects, change the stack defaults, tune the coding rules, and keep the parts that help your AI tools work with better context.

If you use this in your own projects, keep `coding-skills.md` as the canonical source and let the tool-specific files point back to it. That way Claude Code, Codex CLI, Cursor, Windsurf, and GitHub Copilot all follow the same standard without extra setup.

Build honestly. Document clearly. Ship daily.

Built with ❤️ for open source by [Shreyas Pandey](https://github.com/Shreyas-prog108).
