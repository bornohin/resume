# Resume

Working repo for my resume, currently being retargeted toward **Forward Deployed Engineer (FDE)** roles.

| File | What it is |
|---|---|
| `Tom_Islam_Template.docx` | Current resume template |

## What FDE hiring managers look for

1. **Deploying where the customer actually works.** Getting software running inside someone else's environment, including offline, air-gapped or locked-down setups where you can't install whatever you want.
2. **Going from a vague problem to a working prototype fast.** Owning the whole path end to end: understand the problem, build it, ship it, iterate.
3. **Integrating LLMs into real systems.** Retrieval-augmented generation (RAG), tool calling, agents, Model Context Protocol (MCP) servers and evaluations, wired into the data and tools people already use.
4. **Working directly with customers and stakeholders.** Gathering requirements, demoing, handling escalations and explaining technical tradeoffs to people who aren't engineers.

### How my work maps to it

| Signal | Evidence |
|---|---|
| Constrained-environment deployment | [rag-builder](https://github.com/bornohin/rag-builder): fully offline hybrid RAG served over MCP; no sudo, no daemon, no network at query time; offline setup guide for blocked networks |
| Privacy-first, on-device AI | [MinuVault](https://github.com/bornohin/MinuVault): 100% offline finance app with a local LLM (llama.cpp over a JNI bridge), on-device OCR and statement shredding |
| Shipping and distributing tooling | [ai-control-plane](https://github.com/bornohin/ai-control-plane): desktop app (Rust + React) for managing MCP servers, agent skills and model adapters, with a CI release pipeline and auto-updater |
| Stakeholder-facing work | Self-serve evaluation tooling for non-engineers, external hardware-vendor certification, a cross-functional certification program delivered in 7 months against a 2-year estimate |

## TODO

### Resume
- [x] Rewrite the summary toward FDE work
- [x] Add an "LLM Systems" skills line (RAG, hybrid retrieval, MCP, tool calling, on-device inference, evals)
- [x] Add a Selected Projects section built from public repos
- [x] Reorder experience bullets to lead with partner collaboration and stakeholder tooling
- [x] Add location, work authorization, travel and clearance line to the header
- [ ] Keep `Tom_Islam_Template.docx` in sync with the FDE version of the resume

### Projects
- [ ] Replace the default template README in `ai-control-plane` with a real one (what it does, screenshots, install steps)
- [ ] Add measured numbers to `rag-builder`: index size, indexing time, query latency, retrieval hit rate on a test set
- [ ] Add on-device benchmarks to `MinuVault`: tokens/sec, model load time, memory use
- [ ] Record a short demo video for each public project and link it from its README

### Stories and interview prep
- [ ] Write down real examples of customer- or partner-facing work (demos, requirement gathering, escalations)
- [ ] Prepare STAR stories: deploying under constraints, ambiguous requirements, stakeholder disagreement, a fast turnaround
- [ ] Practice a 5-minute live demo of `rag-builder`, from install to first answer
- [ ] Practice a system-design walkthrough of hybrid retrieval and reciprocal rank fusion
