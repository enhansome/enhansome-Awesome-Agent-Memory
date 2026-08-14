# Awesome Agent Memory with stars

<a name="readme-top"></a>

<h1 align="center">🧠 Awesome Agent Memory</h1>

<p align="center">
    A curated map of memory for AI agents — the systems, benchmarks, and research that give LLM and multimodal agents long-term context, persistent recall, and the ability to improve from experience.
</p>

<p align="center">
   👀 <b>Open-source</b> resources (e.g. papers with reproducible code publicly available on Github) are marked in bold font and ranked higher.
</p>

<p align="center">
   <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
   <a href="LICENSE"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License: Apache 2.0"></a>
   <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
   <a href="https://github.com/TeleAI-UAGI/Awesome-Agent-Memory/commits/main"><img src="https://img.shields.io/github/last-commit/TeleAI-UAGI/Awesome-Agent-Memory" alt="Last Commit"></a>
</p>

***

### 🧭 Start Here

| If you want to…                                | Jump to                                                                                                           |
| ---------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Add a memory layer to an agent you're building | [💿 Products](#-products)                                                                                         |
| Choose a benchmark to evaluate a memory system | [📏 Benchmarks](#-benchmarks)                                                                                     |
| Get oriented in the field                      | [📖 Tutorials](#-tutorials) · [📚 Surveys](#-surveys)                                                             |
| Follow research on memory architectures        | [🔤 Nonparametric Memory](#-papers---nonparametric-memory) · [🔢 Parametric Memory](#-papers---parametric-memory) |
| Build agents that learn from experience        | [📈 Memory for Agent Evolution](#-papers---memory-for-agent-evolution)                                            |
| Protect agent memory from poisoning and abuse  | [🔒 Memory Security & Defense](#-memory-security--defense)                                                        |

<details>
  <summary>📋 <b>How this list is curated</b></summary>

* Open-source products are ordered by GitHub star count — an objective, CI-checked popularity signal, not a quality ranking or an endorsement. Products with fewer than 100 stars sit in a collapsed **Emerging projects** section and graduate into the main list once they cross that threshold.
* **Bold** marks resources with reproducible code publicly available.
* Descriptions are factual, not promotional (see the [contributing guide](CONTRIBUTING.md)).
* This list is maintained by [Bloo-Mind AI](https://www.bloo-mind.ai/) and the Ubiquitous AGI team at TeleAI. Entries affiliated with the maintainers are marked with † and follow exactly the same ranking, format, and style rules as every other entry.
* Projects that are inactive, archived, or whose claims are disputed move to the [Archival](#archival) subsection with a neutral status label, links to the evidence, and the date the status was last checked.

</details>

<details>
  <summary>📰 <b>In the News</b></summary>

* 📰 [\[Perplexity (2026-06-18)\] Perplexity launches Brain, a self-improving memory system](https://www.perplexity.ai/hub/blog/self-improving-memory-for-agents)
* 📰 [\[OpenAI (2026-06-04)\] Dreaming: Better memory for a more helpful ChatGPT](https://openai.com/index/chatgpt-memory-dreaming/)
* 📰 [\[Bloo-Mind AI (2026-05-20)\] The Benchmark Theatre: Why Almost Nothing You’ve Read About Agent Memory Scores Is True](https://essays.bloo-mind.ai/posts/2026-05-20-mem-eval/) †
* 📰 [\[Jiayi Weng (2026-05-09)\] Learning Beyond Gradients](https://trinkle23897.github.io/learning-beyond-gradients/)
* 📰 [\[Anthropic (2026-05-08)\] Three key areas Anthropic is working on for their next models](https://www.reddit.com/r/singularity/comments/1t5q53r/three_key_areas_anthropic_is_working_on_for_their/)
* 📰 [\[InfoQ (2026-04-30)\] Cloudflare Announces Agent Memory, a Managed Persistent Memory Service for AI Agents](https://www.infoq.com/news/2026/04/cloudflare-agent-memory-beta/)
* 📰 [\[OpenAI (2026-04-22)\] Chronicle: Build Codex Memories from Recent Screen Context](https://developers.openai.com/codex/memories/chronicle)
  * *Open-Source Alternatives*: [OpenChronicle](https://github.com/Einsia/OpenChronicle) ⭐ 2,726 | 🐛 14 | 🌐 Python | 📅 2026-05-09, [MemScreen](https://github.com/smileformylove/MemScreen) ⭐ 137 | 🐛 0 | 🌐 Python | 📅 2026-06-11
* 📰 [\[a16z (2026-04-22)\] Why We Need Continual Learning](https://a16z.com/why-we-need-continual-learning/)
* 📰 [\[AI Godfather (2026-04-08)\] MemPalace - How Milla Jovovich's AI Project Scammed the Internet](https://www.youtube.com/watch?v=WlxNNvDHJkE)
* 📰 [\[Troy Hua (2026-03-31)\] How Anthropic Built 7 Layers of Memory and a Dreaming System for Claude Code](https://x.com/troyhua/status/2039052328070734102)
* 📰 [\[VelvetShark (2026-03-05)\] OpenClaw Memory Masterclass: The complete guide to agent memory that survives](https://velvetshark.com/openclaw-memory-masterclass)
* 📰 [\[Business Insider (2026-01-08)\] AI still needs a breakthrough in one key area to reach superintelligence, according to those who build it](https://www.businessinsider.com/superintelligent-ai-memory-sam-altman-2026-1)

</details>

***

<details open>
  <summary>🗂️ <b>Table of Contents</b> </summary>
  <ul>
    <li><a href="#-products">💿 Products</a></li>
    <li><a href="#-tutorials">📖 Tutorials</a></li>
    <li><a href="#-surveys">📚 Surveys</a></li>
    <li><a href="#-benchmarks">📏 Benchmarks</a></li>
    <ul>
        <li><a href="#-plain-text-benchmarks">💬 Plain-Text Benchmarks</a></li>
        <li><a href="#-multimodal-benchmarks">🎬 Multimodal Benchmarks</a></li>
        <li><a href="#-dynamic-benchmarks--simulation-environments">🎮 Dynamic Benchmarks & Simulation Environments</a></li>
    </ul>
    <li><a href="#-papers---nonparametric-memory">🔤 Papers - Nonparametric Memory</a></li>
    <ul>
        <li><a href="#-text-memory">📝 Text Memory</a></li>
        <li><a href="#-graph-memory">🌐 Graph Memory</a></li>
        <li><a href="#-multimodal-memory-for-understanding">🎥 Multimodal Memory (for Understanding)</a></li>
        <li><a href="#-multimodal-memory-for-generation">🎥 Multimodal Memory (for Generation)</a></li>
    </ul>
    <li><a href="#-papers---parametric-memory">🔢 Papers - Parametric Memory</a></li>
    <li><a href="#-papers---memory-for-agent-evolution">📈 Papers - Memory for Agent Evolution</a></li>
    <ul>
        <li><a href="#-reinforcement-learning--continual-learning">🧭 Reinforcement Learning & Continual Learning</a></li>
        <li><a href="#-context-engineering--harness-engineering">🧩 Context Engineering & Harness Engineering</a></li>
    </ul>
    <li><a href="#-papers---memory-in-cognitive-science">🔬 Papers - Memory in Cognitive Science</a></li>
    <li><a href="#-memory-security--defense">🔒 Memory Security & Defense</a></li>
    <li><a href="#-articles">📰 Articles</a></li>
    <li><a href="#-workshops">👥 Workshops</a></li>
  </ul>
</details>

<div align="left">

**If you find this page helpful, please give it a ⭐️ — starring also keeps updates in your GitHub feed.**

*🤝 Contributions welcome! Feel free to open an issue or submit a pull request to add papers, fix links, or improve categorization — see the [contributing guide](CONTRIBUTING.md) for entry formats.*

</div>

***

## 💿 Products

### Open-Source

*Ordered by the number of GitHub stars. Products with fewer than 100 stars continue the list inside the collapsed **Emerging projects** section below — they graduate into the main list once they cross that threshold.*

1. **[Claude-Mem (A Plug-in for Claude-Code)](https://claude-mem.ai/)**
   ![Star](https://img.shields.io/github/stars/thedotmack/claude-mem.svg?style=social\&label=Star)
   \[[code](https://github.com/thedotmack/claude-mem) ⭐ 90,677 | 🐛 432 | 🌐 JavaScript | 📅 2026-08-14]
   \[[docs](https://docs.claude-mem.ai/introduction)]
   *Session capture and compression that re-injects past activity into future sessions across coding agents.*

2. **[Mem0](https://mem0.ai/)**
   ![Star](https://img.shields.io/github/stars/mem0ai/mem0.svg?style=social\&label=Star)
   \[[code](https://github.com/mem0ai/mem0) ⭐ 63,219 | 🐛 680 | 🌐 Python | 📅 2026-08-13]
   \[[docs](https://docs.mem0.ai/)]
   \[[paper](https://arxiv.org/abs/2504.19413)]
   \[[blog](https://mem0.ai/blog)]
   *Universal memory layer for AI agents.*

   * **[TeleMem](https://github.com/TeleAI-UAGI/TeleMem) ⭐ 483 | 🐛 1 | 🌐 Python | 📅 2026-08-10** †
     ![Star](https://img.shields.io/github/stars/TeleAI-UAGI/TeleMem.svg?style=social\&label=Star)
     \[[code](https://github.com/TeleAI-UAGI/TeleMem) ⭐ 483 | 🐛 1 | 🌐 Python | 📅 2026-08-10]
     \[[docs](https://teleai-uagi.github.io/telemem/)]
     \[[paper](https://arxiv.org/abs/2601.06037)]
     *API-compatible high-performance drop-in replacement for Mem0 (`import telemem as mem0`); listed as a sub-item of Mem0 rather than ranked by stars. Maintainer-affiliated.*

3. **[Cognee](https://www.cognee.ai/)**
   ![Star](https://img.shields.io/github/stars/topoteretes/cognee.svg?style=social\&label=Star)
   \[[code](https://github.com/topoteretes/cognee) ⭐ 30,007 | 🐛 367 | 🌐 Python | 📅 2026-08-14]
   \[[paper](https://arxiv.org/abs/2505.24478)]
   \[[blog](https://www.cognee.ai/blog)]
   *Memory engine that ingests data into a hybrid graph + vector knowledge graph for cross-session agent recall.*

4. **[Zep (powered by Graphiti)](https://www.getzep.com/)**
   ![Star](https://img.shields.io/github/stars/getzep/graphiti.svg?style=social\&label=Star)
   \[[code](https://github.com/getzep/graphiti) ⭐ 29,902 | 🐛 480 | 🌐 Python | 📅 2026-08-13]
   \[[paper](https://arxiv.org/abs/2501.13956)]
   \[[blog](https://blog.getzep.com/)]
   *Real-time temporal knowledge graphs for AI agents.*

5. **[gbrain](https://github.com/garrytan/gbrain) ⭐ 28,401 | 🐛 433 | 🌐 TypeScript | 📅 2026-08-14**
   ![Star](https://img.shields.io/github/stars/garrytan/gbrain.svg?style=social\&label=Star)
   \[[code](https://github.com/garrytan/gbrain) ⭐ 28,401 | 🐛 433 | 🌐 TypeScript | 📅 2026-08-14]
   *Garry's opinionated OpenClaw/Hermes agent brain.*

6. **[agentmemory](https://www.agent-memory.dev/)**
   ![Star](https://img.shields.io/github/stars/rohitg00/agentmemory.svg?style=social\&label=Star)
   \[[code](https://github.com/rohitg00/agentmemory) ⭐ 26,980 | 🐛 455 | 🌐 TypeScript | 📅 2026-08-10]
   *Persistent memory for AI coding agents.*

7. **[Letta (formerly MemGPT)](https://www.letta.com/)**
   ![Star](https://img.shields.io/github/stars/letta-ai/letta.svg?style=social\&label=Star)
   \[[code](https://github.com/letta-ai/letta) ⭐ 24,231 | 🐛 43 | 🌐 Python | 📅 2026-08-14]
   \[[paper](https://arxiv.org/abs/2310.08560)]
   \[[research](https://www.letta.com/research)]
   \[[blog](https://www.letta.com/blog)]
   *Stateful-agent platform with hierarchical memory that learns and self-improves over time.*

8. **[TencentDB Agent Memory](https://github.com/Tencent/TencentDB-Agent-Memory) ⭐ 21,351 | 🐛 564 | 🌐 TypeScript | 📅 2026-08-11**
   ![Star](https://img.shields.io/github/stars/Tencent/TencentDB-Agent-Memory.svg?style=social\&label=Star)
   \[[code](https://github.com/Tencent/TencentDB-Agent-Memory) ⭐ 21,351 | 🐛 564 | 🌐 TypeScript | 📅 2026-08-11]
   *Fully local long-term memory for AI agents via a 4-tier progressive pipeline, with zero external API dependencies.*

9. **[Hindsight](https://hindsight.vectorize.io/)**
   ![Star](https://img.shields.io/github/stars/vectorize-io/hindsight.svg?style=social\&label=Star)
   \[[code](https://github.com/vectorize-io/hindsight) ⭐ 19,922 | 🐛 104 | 🌐 Python | 📅 2026-08-14]
   \[[paper](https://arxiv.org/abs/2512.12818)]
   *Agent memory layer that learns from interaction feedback to improve recall over time.*

10. **[Context Mode](https://context-mode.com/)**
    ![Star](https://img.shields.io/github/stars/mksglu/context-mode.svg?style=social\&label=Star)
    \[[code](https://github.com/mksglu/context-mode) ⭐ 19,849 | 🐛 150 | 🌐 TypeScript | 📅 2026-08-13]
    *Context-window optimization for AI coding agents — diverts large tool outputs into a locally searchable store and persists session memory across agent platforms via MCP and hooks.*

11. **[Second Me](https://home.second.me/)**
    ![Star](https://img.shields.io/github/stars/mindverse/Second-Me.svg?style=social\&label=Star)
    \[[code](https://github.com/mindverse/Second-Me) ⭐ 15,663 | 🐛 144 | 🌐 Python | 📅 2025-09-30]
    \[[paper](https://arxiv.org/abs/2503.08102)]
    *Personal AI trained on the user to represent them across applications.*

12. **[MemU](https://memu.pro/)**
    ![Star](https://img.shields.io/github/stars/NevaMind-AI/memU.svg?style=social\&label=Star)
    \[[code](https://github.com/NevaMind-AI/memU) ⭐ 14,301 | 🐛 111 | 🌐 Python | 📅 2026-08-12]
    \[[blog](https://memu.pro/blog)]
    *Memory layer for 24/7 proactive agents.*

13. **[EverOS (part of EverMind)](https://evermind-ai.com/)**
    ![Star](https://img.shields.io/github/stars/EverMind-AI/EverOS.svg?style=social\&label=Star)
    \[[code](https://github.com/EverMind-AI/EverOS) ⭐ 12,005 | 🐛 71 | 🌐 Python | 📅 2026-08-13]
    \[[blog](https://evermind-ai.com/blog/)]
    *Toolkit for building, evaluating, and integrating long-term memory in self-evolving agents.*

14. **[MemOS (by MemTensor)](https://memos.openmem.net/)**
    ![Star](https://img.shields.io/github/stars/MemTensor/MemOS.svg?style=social\&label=Star)
    \[[code](https://github.com/MemTensor/MemOS) ⭐ 10,711 | 🐛 103 | 🌐 TypeScript | 📅 2026-08-14]
    \[[paper](https://arxiv.org/abs/2507.03724)]
    *Memory OS for LLM agents with hybrid retrieval and cross-task skill reuse.*

15. **[Honcho](https://honcho.dev/)**
    ![Star](https://img.shields.io/github/stars/plastic-labs/honcho.svg?style=social\&label=Star)
    \[[code](https://github.com/plastic-labs/honcho) ⭐ 6,636 | 🐛 160 | 🌐 Python | 📅 2026-08-13]
    \[[research](https://blog.plasticlabs.ai/research/)]
    \[[blog](https://blog.plasticlabs.ai/)]
    \[[evals](https://evals.honcho.dev/)]
    *Memory library for stateful agents with a focus on user modeling.*

16. **[engram](https://github.com/Gentleman-Programming/engram) ⭐ 5,997 | 🐛 182 | 🌐 Go | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/Gentleman-Programming/engram.svg?style=social\&label=Star)
    \[[code](https://github.com/Gentleman-Programming/engram) ⭐ 5,997 | 🐛 182 | 🌐 Go | 📅 2026-08-13]
    *Persistent memory for AI coding agents — agent-agnostic single Go binary with SQLite + FTS5, exposed via MCP server, HTTP API, CLI, and TUI.*

17. **[MemoryBear](https://www.memorybear.ai/)**
    ![Star](https://img.shields.io/github/stars/SuanmoSuanyangTechnology/MemoryBear.svg?style=social\&label=Star)
    \[[code](https://github.com/SuanmoSuanyangTechnology/MemoryBear) ⭐ 4,992 | 🐛 7 | 🌐 Python | 📅 2026-08-14]
    \[[paper](https://arxiv.org/abs/2512.20651)]
    *Memory framework providing human-like episodic and semantic recall to AI agents.*

18. **[memory-lancedb-pro](https://github.com/CortexReach/memory-lancedb-pro) ⭐ 4,464 | 🐛 54 | 🌐 JavaScript | 📅 2026-08-09**
    ![Star](https://img.shields.io/github/stars/CortexReach/memory-lancedb-pro.svg?style=social\&label=Star)
    \[[code](https://github.com/CortexReach/memory-lancedb-pro) ⭐ 4,464 | 🐛 54 | 🌐 JavaScript | 📅 2026-08-09]
    \[[blog](https://lancedb.com/blog/openclaw-lancedb-memory-layer/)]
    \[[video](https://www.youtube.com/watch?v=bhuGrjuCM_g)]
    *Enhanced [LanceDB](https://lancedb.com/) memory plugin for [OpenClaw](https://openclaw.ai/)*

19. **[OpenMemory](https://openmemory.cavira.app/)**
    ![Star](https://img.shields.io/github/stars/caviraoss/openmemory.svg?style=social\&label=Star)
    \[[code](https://github.com/caviraoss/openmemory) ⭐ 4,432 | 🐛 17 | 🌐 TypeScript | 📅 2026-08-13]
    *Local persistent memory store for LLM apps (Claude Desktop, Copilot, Codex, etc.).*

20. **[MIRIX](https://mirix.io/)**
    ![Star](https://img.shields.io/github/stars/Mirix-AI/MIRIX.svg?style=social\&label=Star)
    \[[code](https://github.com/Mirix-AI/MIRIX) ⭐ 3,482 | 🐛 44 | 🌐 Python | 📅 2026-08-11]
    \[[paper](https://arxiv.org/abs/2507.07957)]
    \[[blog](https://mirix.io/#/blog)]
    *Multi-agent personal assistant that captures on-screen activity and consolidates it into structured memory.*

21. **[MemMachine](https://memmachine.ai/)**
    ![Star](https://img.shields.io/github/stars/MemMachine/MemMachine.svg?style=social\&label=Star)
    \[[code](https://github.com/MemMachine/MemMachine) ⭐ 3,347 | 🐛 86 | 🌐 Python | 📅 2026-08-13]
    \[[blog](https://memmachine.ai/blog/)]
    *Interoperable memory layer providing extensible storage and retrieval primitives for AI agents.*

22. **[Memobase](https://docs.memobase.io/)**
    ![Star](https://img.shields.io/github/stars/memodb-io/memobase.svg?style=social\&label=Star)
    \[[code](https://github.com/memodb-io/memobase) ⭐ 2,842 | 🐛 30 | 🌐 Python | 📅 2026-01-11]
    *User profile-based long-term memory for AI chatbot applications.*

23. **[Memanto](https://memanto.ai/)** ![Star](https://img.shields.io/github/stars/moorcheh-ai/memanto.svg?style=social\&label=Star)
    \[[code](https://github.com/moorcheh-ai/memanto) ⭐ 1,796 | 🐛 122 | 🌐 Python | 📅 2026-08-13]
    \[[paper](https://arxiv.org/abs/2604.22085)]
    \[[docs](https://docs.memanto.ai)]
    *Typed semantic memory with `remember`/`recall`/`answer` operations and information-theoretic retrieval.*

24. **[LangMem](https://langchain-ai.github.io/langmem/)**
    ![Star](https://img.shields.io/github/stars/langchain-ai/langmem.svg?style=social\&label=Star)
    \[[code](https://github.com/langchain-ai/langmem) ⭐ 1,606 | 🐛 59 | 🌐 Python | 📅 2026-08-11]
    \[[blog](https://blog.langchain.com/)]
    *LangChain's memory primitives for storing, recalling, and managing agent state in LangGraph workflows.*

25. **[Puppyone](https://www.puppyone.ai)**
    ![Star](https://img.shields.io/github/stars/puppyone-ai/puppyone.svg?style=social\&label=Star)
    \[[code](https://github.com/puppyone-ai/puppyone) ⭐ 1,326 | 🐛 26 | 🌐 TypeScript | 📅 2026-08-02]
    \[[docs](https://www.puppyone.ai/doc)]
    *Filesystem-shaped agent memory with auto-versioning, per-agent ACLs, and data connectors; accessible via MCP/REST/CLI.*

26. **[Mem9](https://mem9.ai/)**
    ![Star](https://img.shields.io/github/stars/mem9-ai/mem9.svg?style=social\&label=Star)
    \[[code](https://github.com/mem9-ai/mem9) ⭐ 1,186 | 🐛 88 | 🌐 TypeScript | 📅 2026-08-12]
    \[[blog](https://addozhang.medium.com/keep-memory-local-building-a-private-openclaw-memory-hub-with-mem9-tidb-5b305345b40a)]
    *Local private memory hub for OpenClaw and similar coding agents.*

27. **[Omnigraph](https://github.com/ModernRelay/omnigraph) ⭐ 1,056 | 🐛 21 | 🌐 Rust | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/ModernRelay/omnigraph.svg?style=social\&label=Star)
    \[[code](https://github.com/ModernRelay/omnigraph) ⭐ 1,056 | 🐛 21 | 🌐 Rust | 📅 2026-08-13]
    *Object-storage-native graph engine for agent memory with git-style branch/merge workflows.*

28. **[PowerMem](https://www.powermem.ai)**
    ![Star](https://img.shields.io/github/stars/oceanbase/powermem.svg?style=social\&label=Star)
    \[[code](https://github.com/oceanbase/powermem) ⭐ 859 | 🐛 7 | 🌐 Python | 📅 2026-08-14]
    *Persistent, self-evolving memory for AI agents — hybrid vector/full-text/graph retrieval with LLM-driven extraction, Ebbinghaus-style decay, and two-layer Experience + Skill distillation; from the OceanBase team.*

29. **[CodeAlmanac](https://github.com/AlmanacCode/codealmanac) ⭐ 799 | 🐛 42 | 🌐 TypeScript | 📅 2026-07-25**
    ![Star](https://img.shields.io/github/stars/AlmanacCode/codealmanac.svg?style=social\&label=Star)
    \[[code](https://github.com/AlmanacCode/codealmanac) ⭐ 799 | 🐛 42 | 🌐 TypeScript | 📅 2026-07-25]
    *Repo-local Markdown wiki for AI coding agents that preserves project conversations, decisions, and implementation context.*

30. **[projectmem](https://projectmem.dev)**
    ![Star](https://img.shields.io/github/stars/riponcm/projectmem.svg?style=social\&label=Star)
    \[[code](https://github.com/riponcm/projectmem) ⭐ 657 | 🐛 1 | 🌐 Python | 📅 2026-08-06]
    \[[docs](https://projectmem.dev/guide)]
    \[[paper](https://arxiv.org/abs/2606.12329)]
    *Local-first, event-sourced memory and judgment layer for AI coding agents: an append-only event log served via MCP, plus a pre-commit gate that warns before repeating a failed fix.*

31. **[Memorix](https://github.com/AVIDS2/memorix) ⭐ 632 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/AVIDS2/memorix.svg?style=social\&label=Star)
    \[[code](https://github.com/AVIDS2/memorix) ⭐ 632 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-13]
    *Local-first cross-agent memory layer for coding agents via MCP — SQLite-backed project memory with observation, reasoning, and git-derived fact types, plus task-lensed context briefs.*

32. **[Compartment](https://github.com/MaxFreedomPollard/Compartment) ⭐ 627 | 🐛 0 | 🌐 Python | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/MaxFreedomPollard/Compartment.svg?style=social\&label=Star)
    \[[code](https://github.com/MaxFreedomPollard/Compartment) ⭐ 627 | 🐛 0 | 🌐 Python | 📅 2026-08-13]
    *Offline, encrypted-at-rest vector memory for agents via MCP server, Python, or CLI; AEAD-encrypted embeddings, hybrid recall, per-record crypto-shred deletion, hash-chained audit log.*

33. **[HMS (Holographic Memory System)](https://github.com/Shadow-Weave/HMS) ⭐ 605 | 🐛 0 | 🌐 Python | 📅 2026-08-05**
    ![Star](https://img.shields.io/github/stars/Shadow-Weave/HMS.svg?style=social\&label=Star)
    \[[code](https://github.com/Shadow-Weave/HMS) ⭐ 605 | 🐛 0 | 🌐 Python | 📅 2026-08-05]
    *Long-term memory QA framework that wraps OpenAI clients with automatic recall and retain, PostgreSQL-backed, evaluated on LongMemEval.*

34. **[Vestige](https://github.com/samvallad33/vestige) ⭐ 602 | 🐛 11 | 🌐 Rust | 📅 2026-08-12**
    ![Star](https://img.shields.io/github/stars/samvallad33/vestige.svg?style=social\&label=Star)
    \[[code](https://github.com/samvallad33/vestige) ⭐ 602 | 🐛 11 | 🌐 Rust | 📅 2026-08-12]
    \[[release](https://github.com/samvallad33/vestige/releases/tag/v2.1.23) ⭐ 602 | 🐛 11 | 🌐 Rust | 📅 2026-08-12]
    *Local-first cognitive memory MCP server for coding agents, with FSRS-6 decay, spreading activation, active suppression, Receipt Lock, and an inspectable dashboard.*

35. **[MemClaw (Caura)](https://memclaw.net/)**
    ![Star](https://img.shields.io/github/stars/caura-ai/caura-memclaw.svg?style=social\&label=Star)
    \[[code](https://github.com/caura-ai/caura-memclaw) ⭐ 430 | 🐛 37 | 🌐 Python | 📅 2026-08-13]
    \[[blog](https://memclaw.net/blog)]
    *Governed shared memory for AI agent fleets — cross-agent knowledge sharing with permissions, audit trails, and self-learning.*

36. **[MisakaNet](https://github.com/Ikalus1988/MisakaNet) ⭐ 397 | 🐛 27 | 🌐 Python | 📅 2026-08-14**
    ![Star](https://img.shields.io/github/stars/Ikalus1988/MisakaNet.svg?style=social\&label=Star)
    \[[code](https://github.com/Ikalus1988/MisakaNet) ⭐ 397 | 🐛 27 | 🌐 Python | 📅 2026-08-14]
    \[[wiki](https://github.com/Ikalus1988/MisakaNet/wiki) ⭐ 397 | 🐛 27 | 🌐 Python | 📅 2026-08-14]
    *Git-based distributed swarm memory; agents share lessons across nodes via GitHub Issues.*

37. **[Statewave](https://statewave.ai/)**
    ![Star](https://img.shields.io/github/stars/smaramwbc/statewave.svg?style=social\&label=Star)
    \[[code](https://github.com/smaramwbc/statewave) ⭐ 313 | 🐛 10 | 🌐 Python | 📅 2026-08-13]
    \[[docs](https://github.com/smaramwbc/statewave-docs) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-07-28]
    \[[blog](https://www.statewave.ai/blog)]
    *Open-source memory runtime for AI agents serving reproducible, provenance-tagged context bundles instead of query-time retrieval; self-hosted on Postgres + pgvector with Python/TypeScript SDKs.*

38. **[Mnemory](https://github.com/fpytloun/mnemory) ⭐ 268 | 🐛 1 | 🌐 Python | 📅 2026-06-09** ![Star](https://img.shields.io/github/stars/fpytloun/mnemory.svg?style=social\&label=Star)
    \[[code](https://github.com/fpytloun/mnemory) ⭐ 268 | 🐛 1 | 🌐 Python | 📅 2026-06-09]
    *Multi-type agent memory (facts, preferences, episodic) with TTLs, user/agent scoping, and an MCP server.*

39. **[OMEGA](https://omegamax.co)** ![Star](https://img.shields.io/github/stars/omega-memory/omega-memory.svg?style=social\&label=Star)
    \[[code](https://github.com/omega-memory/omega-memory) ⭐ 202 | 🐛 7 | 🌐 Python | 📅 2026-08-14]
    \[[blog](https://omegamax.co/blog)]
    *MCP server exposing 25 memory tools for AI coding agents.*

40. **[Memov](https://www.memov.ai/)**
    ![Star](https://img.shields.io/github/stars/memovai/memov.svg?style=social\&label=Star)
    \[[code](https://github.com/memovai/memov) ⭐ 191 | 🐛 13 | 🌐 Python | 📅 2026-02-05]
    *Git-based, traceable memory layer for Claude Code.*

41. **[CommonGround Kernel](https://github.com/Intelligent-Internet/CommonGround) ⭐ 147 | 🐛 1 | 🌐 Python | 📅 2026-05-20**
    ![Star](https://img.shields.io/github/stars/Intelligent-Internet/CommonGround.svg?style=social\&label=Star)
    \[[code](https://github.com/Intelligent-Internet/CommonGround) ⭐ 147 | 🐛 1 | 🌐 Python | 📅 2026-05-20]
    *PostgreSQL-backed shared work-record substrate for human-agent and multi-agent systems, with durable handoff facts, causal lineage, and pull-first recovery across runtimes.*

<details>
  <summary>🌱 <b>Emerging projects</b> — open-source products with fewer than 100 GitHub stars, same format and ordering (click to expand)</summary>

42. **[taOSmd](https://github.com/jaylfc/taosmd) ⭐ 75 | 🐛 47 | 🌐 Python | 📅 2026-08-14**
    ![Star](https://img.shields.io/github/stars/jaylfc/taosmd.svg?style=social\&label=Star)
    \[[code](https://github.com/jaylfc/taosmd) ⭐ 75 | 🐛 47 | 🌐 Python | 📅 2026-08-14]
    \[[benchmarks](https://github.com/jaylfc/taosmd/blob/master/docs/benchmarks.md) ⭐ 75 | 🐛 47 | 🌐 Python | 📅 2026-08-14]
    *Local-first, offline agent memory: an append-only transcript yields a typed temporal knowledge graph with source-grounded, verifier-checked facts and hybrid retrieval, tuned for small local models.*

43. **[Synap](https://maximem.ai)**
    ![Star](https://img.shields.io/github/stars/maximem-ai/maximem_synap_sdk.svg?style=social\&label=Star)
    \[[code](https://github.com/maximem-ai/maximem_synap_sdk) ⭐ 60 | 🐛 9 | 🌐 Python | 📅 2026-08-10]
    \[[docs](https://docs.maximem.ai)]
    *Long-term memory layer that extracts facts, preferences, episodes, and temporal events from conversations; integrates with most major agent frameworks.*

44. **[widemem-ai](https://widemem.ai)**
    ![Star](https://img.shields.io/github/stars/remete618/widemem-ai.svg?style=social\&label=Star)
    \[[code](https://github.com/remete618/widemem-ai) ⭐ 48 | 🐛 7 | 🌐 Python | 📅 2026-08-01]
    *Lightweight memory layer with importance scoring, temporal decay, and 3-tier hierarchy.*

45. **[Wenlan](https://wenlan.app/)**
    ![Star](https://img.shields.io/github/stars/7xuanlu/wenlan.svg?style=social\&label=Star)
    \[[code](https://github.com/7xuanlu/wenlan) ⭐ 47 | 🐛 1 | 🌐 Rust | 📅 2026-08-13]
    \[[docs](https://wenlan.app/docs)]
    *Local-first AI knowledge base and LLM wiki that distills agent work into source-cited pages and serves them to MCP clients.*

46. **[Mimir](https://github.com/Perseus-Computing-LLC/mimir) ⭐ 47 | 🐛 4 | 🌐 Rust | 📅 2026-08-14**
    ![Star](https://img.shields.io/github/stars/Perseus-Computing-LLC/mimir.svg?style=social\&label=Star)
    \[[code](https://github.com/Perseus-Computing-LLC/mimir) ⭐ 47 | 🐛 4 | 🌐 Rust | 📅 2026-08-14]
    *MCP-native persistent memory for agents as a single Rust binary — embedded SQLite with FTS5 + vector hybrid search, AES-256-GCM encryption at rest, fully local.*

47. **[memclaw (Felo)](https://memclaw.me)**
    ![Star](https://img.shields.io/github/stars/Felo-Inc/memclaw.svg?style=social\&label=Star)
    \[[code](https://github.com/Felo-Inc/memclaw) ⭐ 37 | 🐛 1 | 🌐 JavaScript | 📅 2026-04-23]
    *Persistent project memory for AI coding agents — isolated per-project workspaces, a web dashboard to review what the agent remembers, and team collaboration.*

48. **[Mi-Memory](https://darwin-agent.github.io/Mi-Memory/)**
    ![Star](https://img.shields.io/github/stars/Darwin-Agent/Mi-Memory.svg?style=social\&label=Star)
    \[[code](https://github.com/Darwin-Agent/Mi-Memory) ⭐ 26 | 🐛 0 | 🌐 HTML | 📅 2026-07-23]
    \[[docs](https://darwin-agent.github.io/Mi-Memory/)]
    \[[paper](https://arxiv.org/abs/2607.18975)]
    *Lifecycle memory framework for personal assistant agents from Xiaomi's Darwin Agent team; multi-source user state with provenance, editable correction and forgetting, device-adaptive deployment.*

49. **[ZenBrain](https://zensation.ai/en)**
    ![Star](https://img.shields.io/github/stars/zensation-ai/zenbrain.svg?style=social\&label=Star)
    \[[code](https://github.com/zensation-ai/zenbrain) ⭐ 20 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-09]
    \[[paper](https://arxiv.org/abs/2604.23878)]
    *Neuroscience-inspired 7-layer memory architecture for autonomous agents in zero-dependency TypeScript, with FSRS spaced repetition, Hebbian learning, and sleep-cycle consolidation.*

50. **[Data Olympus](https://github.com/knaisoma/data-olympus) ⭐ 18 | 🐛 23 | 🌐 Python | 📅 2026-08-12**
    ![Star](https://img.shields.io/github/stars/knaisoma/data-olympus.svg?style=social\&label=Star)
    \[[code](https://github.com/knaisoma/data-olympus) ⭐ 18 | 🐛 23 | 🌐 Python | 📅 2026-08-12]
    *Governed project memory for AI coding agents: agents propose learnings, humans promote them, and MCP retrieval serves only in-force knowledge after validity and supersession checks.*

51. **[Mnemoverse](https://mnemoverse.com)**
    ![Star](https://img.shields.io/github/stars/mnemoverse/mcp-memory-server.svg?style=social\&label=Star)
    \[[code](https://github.com/mnemoverse/mcp-memory-server) ⭐ 17 | 🐛 15 | 🌐 TypeScript | 📅 2026-08-13]
    *Persistent memory API for agents over MCP: scores importance on write, builds Hebbian associations, and re-ranks recall from outcome feedback; managed engine, open MCP client.*

52. **[GoodMemory](https://github.com/hjqcan/GoodMemory) ⭐ 16 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/hjqcan/GoodMemory.svg?style=social\&label=Star)
    \[[code](https://github.com/hjqcan/GoodMemory) ⭐ 16 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-13]
    \[[docs](https://github.com/hjqcan/GoodMemory#quickstart-codex-or-claude-code-memory) ⭐ 16 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-13]
    *Local-first, auditable memory layer for AI agents and coding hosts, with durable SQLite, embedding-free recall, MCP access, and opt-in governed writeback.*

53. **[A3M Router](https://github.com/Das-rebel/a3m-router) ⭐ 14 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-14**
    ![Star](https://img.shields.io/github/stars/Das-rebel/a3m-router.svg?style=social\&label=Star)
    \[[code](https://github.com/Das-rebel/a3m-router) ⭐ 14 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-14]
    *Multi-model LLM router with persistent memory (MemoryTree), cross-session context-window management, conversation memory with semantic recall, and ObsidianVault integration.*

54. **[Tree Ring Memory](https://terminallylazy.github.io/Tree-Ring-Memory/)**
    ![Star](https://img.shields.io/github/stars/TerminallyLazy/Tree-Ring-Memory.svg?style=social\&label=Star)
    \[[code](https://github.com/TerminallyLazy/Tree-Ring-Memory) ⭐ 12 | 🐛 1 | 🌐 Rust | 📅 2026-07-23]
    *Local-first memory lifecycle for AI agents with a Rust CLI, SQLite/FTS recall, audit, forgetting, consolidation, and Ratatui TUI.*

55. **[Agentic Task System](https://github.com/renezander030/agentic-task-system) ⭐ 10 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-09**
    ![Star](https://img.shields.io/github/stars/renezander030/agentic-task-system.svg?style=social\&label=Star)
    \[[code](https://github.com/renezander030/agentic-task-system) ⭐ 10 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-09]
    \[[npm](https://www.npmjs.com/package/@reneza/ats-cli)]
    *Agent-native context layer over your existing task app (TickTick; Notion/Obsidian planned), exposing hybrid retrieval over tasks/notes to agents via a CLI with pluggable storage adapters.*

56. **[FluctlightDB](https://github.com/voxmastery/FluctlightDB) ⭐ 7 | 🐛 1 | 🌐 Python | 📅 2026-08-06**
    ![Star](https://img.shields.io/github/stars/voxmastery/FluctlightDB.svg?style=social\&label=Star)
    \[[code](https://github.com/voxmastery/FluctlightDB) ⭐ 7 | 🐛 1 | 🌐 Python | 📅 2026-08-06]
    \[[paper](https://doi.org/10.5281/zenodo.20949890)]
    *Embedded database engine for AI agents with `experience()`/`activate()` API and reproducible LoCoMo evaluation.*

57. **[archon-memory-core](https://github.com/atw4757-byte/archon-memory-core) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-04-22**
    ![Star](https://img.shields.io/github/stars/atw4757-byte/archon-memory-core.svg?style=social\&label=Star)
    \[[code](https://github.com/atw4757-byte/archon-memory-core) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-04-22]
    *Local-first agent memory with nightly consolidation, active forgetting, and salience scoring.*

58. **[Lians agent memory](https://www.lians.ai/)**
    ![Star](https://img.shields.io/github/stars/Lians-ai/Lians.svg?style=social\&label=Star)
    \[[code](https://github.com/Lians-ai/Lians) ⭐ 6 | 🐛 10 | 🌐 Python | 📅 2026-08-14]
    \[[benchmark](https://github.com/Lians-ai/Lians/blob/master/docs/benchmark.md) ⭐ 6 | 🐛 10 | 🌐 Python | 📅 2026-08-14]
    *Bitemporal agent memory with deterministic supersession, point-in-time recall, MCP access, audit trails, and local SQLite or PostgreSQL storage.*

59. **[inspeximus (formerly mnemo)](https://dancenitra.github.io/inspeximus/)**
    ![Star](https://img.shields.io/github/stars/DanceNitra/inspeximus.svg?style=social\&label=Star)
    \[[code](https://github.com/DanceNitra/inspeximus) ⭐ 5 | 🐛 1 | 🌐 Python | 📅 2026-08-13]
    \[[pypi](https://pypi.org/project/inspeximus/)]
    *Zero-dependency memory layer and MCP server with value-ranked recall, per-type decay, keyed supersession, revert-based correction, signed provenance, tamper-evident receipts, and cross-store erasure.*

60. **[Agent Knowledge Cycle](https://github.com/shimo4228/agent-knowledge-cycle) ⭐ 3 | 🐛 0 | 📅 2026-08-07**
    ![Star](https://img.shields.io/github/stars/shimo4228/agent-knowledge-cycle.svg?style=social\&label=Star)
    \[[code](https://github.com/shimo4228/agent-knowledge-cycle) ⭐ 3 | 🐛 0 | 📅 2026-08-07]
    \[[paper](https://doi.org/10.5281/zenodo.20578272)]
    *Six-phase knowledge cycle specification (ADRs, JSON schemas, reference implementation) that turns coding-agent sessions into persistent skills, rules, and memory.*

61. **[Talamus](https://ampres-ai.github.io/talamus/)**
    ![Star](https://img.shields.io/github/stars/ampres-ai/talamus.svg?style=social\&label=Star)
    \[[code](https://github.com/ampres-ai/talamus) ⭐ 3 | 🐛 6 | 🌐 Python | 📅 2026-08-05]
    \[[docs](https://ampres-ai.github.io/talamus/)]
    \[[benchmarks](https://ampres-ai.github.io/talamus/benchmarks/)]
    \[[pypi](https://pypi.org/project/talamus/)]
    *Local-first agent memory that stores source-grounded Markdown, preserves bitemporal history and provenance, and exposes search, recall, and review-gated correction through MCP.*

62. **[RE-call](https://github.com/GiulioDER/RE-call) ⭐ 3 | 🐛 9 | 🌐 Python | 📅 2026-08-13**
    ![Star](https://img.shields.io/github/stars/GiulioDER/RE-call.svg?style=social\&label=Star)
    \[[code](https://github.com/GiulioDER/RE-call) ⭐ 3 | 🐛 9 | 🌐 Python | 📅 2026-08-13]
    \[[docs](https://github.com/GiulioDER/RE-call/blob/master/docs/USING_WITH_CLAUDE.md) ⭐ 3 | 🐛 9 | 🌐 Python | 📅 2026-08-13]
    \[[benchmarks](https://github.com/GiulioDER/RE-call/blob/master/results/FINDINGS.md) ⭐ 3 | 🐛 9 | 🌐 Python | 📅 2026-08-13]
    *Postgres plus pgvector memory retrieval for AI agents, with provenance, trust verdicts, tenant isolation, MCP access, and abstention when evidence is insufficient.*

63. **[PackRat](https://github.com/kevdogg102396-afk/packrat) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-04-17**
    ![Star](https://img.shields.io/github/stars/kevdogg102396-afk/packrat.svg?style=social\&label=Star)
    \[[code](https://github.com/kevdogg102396-afk/packrat) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-04-17]
    *Auto-learning codebook compression that shrinks agent context files while keeping them LLM-readable.*

64. **[sqlite-graph-memory](https://github.com/Palo-Alto-AI-Research-Lab/sqlite-graph-memory) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-10**
    ![Star](https://img.shields.io/github/stars/Palo-Alto-AI-Research-Lab/sqlite-graph-memory.svg?style=social\&label=Star)
    \[[code](https://github.com/Palo-Alto-AI-Research-Lab/sqlite-graph-memory) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-10]
    *Graph RAG memory for agents over a markdown vault: dense retrieval, hand-curated wikilink 1-hop expansion, cross-encoder rerank, per-turn SQLite ledger.*

65. **[kgai](https://kgai.dev)**
    ![Star](https://img.shields.io/github/stars/kgaidev/kgai.svg?style=social\&label=Star)
    \[[code](https://github.com/kgaidev/kgai) ⭐ 1 | 🐛 0 | 🌐 Go | 📅 2026-08-07]
    *Local-first immutable knowledge graph of engineering decisions for AI coding agents; superseded decisions and rejected approaches stay queryable; embedded graph DB, opt-in team sync.*

66. **[memgres](https://github.com/mozgsml/memgres) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-31**
    ![Star](https://img.shields.io/github/stars/mozgsml/memgres.svg?style=social\&label=Star)
    \[[code](https://github.com/mozgsml/memgres) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-31]
    *Versioned document memory for AI agents over one Postgres; lexical or semantic recall, diff-based history, git-blame line attribution, GDPR-erasable, multi-tenant via MCP/HTTP.*

67. **[ReFind](https://github.com/imlrz/ReFind) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-14**
    ![Star](https://img.shields.io/github/stars/imlrz/ReFind.svg?style=social\&label=Star)
    \[[code](https://github.com/imlrz/ReFind) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-14]
    *Agentic long-term memory retriever that plans iterative searches over a conversation-level BM25 index and returns contextual evidence blocks; #2 on the Agent Memory Leaderboard academic textual track (2026-08).*

68. **[FlowGrid AML Retriever](https://github.com/dlxeva/flowgrid-aml-retriever) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-12**
    ![Star](https://img.shields.io/github/stars/dlxeva/flowgrid-aml-retriever.svg?style=social\&label=Star)
    \[[code](https://github.com/dlxeva/flowgrid-aml-retriever) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-12]
    *Deterministic, evidence-first Add/Search retriever that stores every original message and returns ranked source evidence with traceable retrieval views; #8 on the Agent Memory Leaderboard academic textual track (2026-08).*

69. **[Akephalos](https://github.com/sunnja69/akephalos) ⭐ 0 | 🐛 16 | 🌐 JavaScript | 📅 2026-08-03**
    ![Star](https://img.shields.io/github/stars/sunnja69/akephalos.svg?style=social\&label=Star)
    \[[code](https://github.com/sunnja69/akephalos) ⭐ 0 | 🐛 16 | 🌐 JavaScript | 📅 2026-08-03]
    *Local-first, markdown-based portable agent profile (preferences, rules, durable memories) synced across agents via plain files and Git.*

70. **[溯忆 (Suyi)](https://github.com/xiaofanliu525-ctrl/suyi-memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-30**
    ![Star](https://img.shields.io/github/stars/xiaofanliu525-ctrl/suyi-memory.svg?style=social\&label=Star)
    \[[code](https://github.com/xiaofanliu525-ctrl/suyi-memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-30]
    *Dual-temporal memory engine for AI agents — SQLite-backed, zero-dependency, Ebbinghaus-decayed fact storage with skill crystallization.*

71. **[Panella](https://panella.tech)**
    ![Star](https://img.shields.io/github/stars/panellatech/panella.svg?style=social\&label=Star)
    \[[code](https://github.com/panellatech/panella) ⭐ 0 | 🐛 18 | 🌐 Python | 📅 2026-08-02]
    *Self-hosted governed memory over MCP; agent writes become durable only after human approval with verifiable receipts; Apache-2.0.*

72. **[InvMem](https://github.com/wenxiaof345-ctrl/vanilla-rag-memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-11**
    ![Star](https://img.shields.io/github/stars/wenxiaof345-ctrl/vanilla-rag-memory.svg?style=social\&label=Star)
    \[[code](https://github.com/wenxiaof345-ctrl/vanilla-rag-memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-11]
    *Vanilla RAG baseline (chunking, embeddings, FAISS/SQLite vector store) behind a synchronous Add/Search API; #1 on the Agent Memory Leaderboard academic textual track (2026-08).*

73. **[ActiveMemoryIndex](https://github.com/linxuhao/ActiveMemoryIndex) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-09**
    ![Star](https://img.shields.io/github/stars/linxuhao/ActiveMemoryIndex.svg?style=social\&label=Star)
    \[[code](https://github.com/linxuhao/ActiveMemoryIndex) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-09]
    *Stores memories twice — verbatim timestamped turns and atomic first-person facts — and retrieves by matching the log's own first-person register; #3 on the Agent Memory Leaderboard academic textual track (2026-08).*

74. **[Hybrid Memory Search](https://github.com/cydd-1972/hybrid_search) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-12**
    ![Star](https://img.shields.io/github/stars/cydd-1972/hybrid_search.svg?style=social\&label=Star)
    \[[code](https://github.com/cydd-1972/hybrid_search) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-12]
    *Local hybrid-retrieval memory service with per-user isolation, synchronous embedding on write, and BM25 + dense fused ranking; #4 on the Agent Memory Leaderboard academic textual track (2026-08).*

75. **[ChronoHybridMem](https://github.com/Tin11Mn/chrono-hybrid-mem) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-08-11**
    ![Star](https://img.shields.io/github/stars/Tin11Mn/chrono-hybrid-mem.svg?style=social\&label=Star)
    \[[code](https://github.com/Tin11Mn/chrono-hybrid-mem) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-08-11]
    *Evidence-only textual memory over SQLite FTS5 with optional LLM fact extraction and multi-route candidate recall; #5 on the Agent Memory Leaderboard academic textual track (2026-08).*

76. **[Hybrid Episodic Memory](https://github.com/tlysanhuo/agent-memory-challenge) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-07**
    ![Star](https://img.shields.io/github/stars/tlysanhuo/agent-memory-challenge.svg?style=social\&label=Star)
    \[[code](https://github.com/tlysanhuo/agent-memory-challenge) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-07]
    *Fully deterministic memory service fusing BM25 and dense retrieval over raw conversational turns via weighted reciprocal rank fusion, with no LLM in the memory path; #6 on the Agent Memory Leaderboard academic textual track (2026-08).*

77. **[Chronicle Memory](https://github.com/simple-boy/Chronicle-Memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-05**
    ![Star](https://img.shields.io/github/stars/simple-boy/Chronicle-Memory.svg?style=social\&label=Star)
    \[[code](https://github.com/simple-boy/Chronicle-Memory) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-05]
    *Evidence-only memory over SQLite with a hybrid lexical scorer adding phrase, temporal, and session-diversity bonuses; #7 on the Agent Memory Leaderboard academic textual track (2026-08).*

78. **[MemoryAgent](https://github.com/llLAlisa/memory-agent-submission) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-06**
    ![Star](https://img.shields.io/github/stars/llLAlisa/memory-agent-submission.svg?style=social\&label=Star)
    \[[code](https://github.com/llLAlisa/memory-agent-submission) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-06]
    *FastAPI + ChromaDB memory system with local sentence-transformers embeddings and similarity-based write deduplication; #9 (as LLLMemoryAgent) on the Agent Memory Leaderboard academic textual track (2026-08).*

79. **[AML Memory MVP](https://github.com/0xboyu/aml-memory-mvp) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-08-12**
    ![Star](https://img.shields.io/github/stars/0xboyu/aml-memory-mvp.svg?style=social\&label=Star)
    \[[code](https://github.com/0xboyu/aml-memory-mvp) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-08-12]
    *Evidence-only retriever indexing English and CJK text with SQLite FTS5 plus character n-grams, typo-tolerant semantic retrieval, and conversation-neighbor expansion; #10 on the Agent Memory Leaderboard academic textual track (2026-08).*

</details>

### Closed-Source

* [Supermemory](https://supermemory.ai/)
  \[[partial-code](https://github.com/supermemoryai/supermemory) ⭐ 28,910 | 🐛 109 | 🌐 TypeScript | 📅 2026-08-14]
  \[[blog](https://supermemory.ai/blog)]

* [screenpipe](https://screenpipe.com)
  \[[source-available](https://github.com/screenpipe/screenpipe) ⭐ 20,944 | 🐛 112 | 🌐 Rust | 📅 2026-08-14]
  \[[license](https://github.com/screenpipe/screenpipe/blob/main/LICENSE.md) ⭐ 20,944 | 🐛 112 | 🌐 Rust | 📅 2026-08-14]
  \[[docs](https://docs.screenpi.pe)]
  *Local-first work memory that captures screen, audio, input, browser, and meeting context for search and agent retrieval.*

* [MemoraX](https://memorax.ai/)
  \[[spec](https://memorax.ai/spec/)]
  \[[partial-code](https://github.com/memorax-ai/memorax-code) ⭐ 527 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-13]
  *Memory layer for long-horizon agents from MemoraX AI; core system is API-only, with an open-source coding-memory plugin; #1 on the Agent Memory Leaderboard industry textual track (2026-08).*

* [AccInt](https://accint.xyz)
  \[[partial-code](https://github.com/maxbaluev/accreted-intelligence) ⭐ 6 | 🐛 2 | 🌐 Shell | 📅 2026-07-05]
  *Local-first MCP Work Model for coding agents that retrieves scored memory, records actions, and credits real outcomes; engine is a closed-source binary.*

* [Threadline](https://threadline.to)
  \[[partial-code](https://github.com/vidursharma202-del/threadline-mcp) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-05-26]
  \[[schema](https://github.com/vidursharma202-del/context-schema) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-07-21]
  \[[docs](https://threadline.to/docs)]

* [MemoryLake](https://www.memorylake.ai/en)
  \[[blog](https://www.memorylake.ai/en/blogs)]

* [Memories.ai](https://memories.ai/)
  \[[research](https://memories.ai/research)]
  \[[paper](https://memories.ai/research/Camera)]
  \[[blog](https://memories.ai/blogs)]

* [Macaron Mind Lab](https://macaron.im/mindlab)
  \[[blog](https://macaron.im/mindlab/research)]
  \[[paper](https://macaron.im/mindlab/publications)]

* [Mem 2.0](https://get.mem.ai/)
  \[[blog](https://get.mem.ai/blog)]

* [M-Flow](https://m-flow.ai/)

* [TwinMind](https://twinmind.com/)
  \[[blog](https://twinmind.com/blogs)]

* [Penfield](https://www.penfield.app/)
  \[[blog](https://penfieldlabs.substack.com/)]

* [Sonzai](https://sonz.ai/)

* [Remio](https://remio.ai/)
  *Local-first personal knowledge base that indexes files, webpages, recordings, notes, emails, and messages for agent retrieval via search and RAG.*

* [Agentage Memory](https://memory.agentage.io)
  *Remote MCP memory server (OAuth 2.1 + PKCE + DCR) giving Claude, Cursor, and ChatGPT one shared markdown memory mirrored locally as files you own.*

### Archival

*Projects that are inactive or whose claims have been disputed by third parties. Status labels link to the evidence and note when the status was last checked.*

* [MemPalace](https://github.com/MemPalace/mempalace) ⭐ 58,355 | 🐛 695 | 🌐 Python | 📅 2026-08-13 ⚠️ Disputed (third-party critiques challenge the project's core claims; last checked 2026-07)
  \[[code](https://github.com/milla-jovovich/mempalace) ⭐ 58,355 | 🐛 695 | 🌐 Python | 📅 2026-08-13]
  \[[critique1](https://www.youtube.com/watch?v=WlxNNvDHJkE), [critique2](https://penfieldlabs.substack.com/p/milla-jovovich-just-released-an-ai)]
  *Developed by actress [Milla Jovovich](https://en.wikipedia.org/wiki/Milla_Jovovich) and her friends*

* [Memvid](https://www.memvid.com/) ⚠️ Disputed (technical critique raised in GitHub issues, since deleted but archived; last checked 2026-07)
  \[[code](https://github.com/Olow304/memvid) ⭐ 16,216 | 🐛 34 | 🌐 Rust | 📅 2026-07-14]
  \[[critique (archived)](https://web.archive.org/web/20250807093442/https://github.com/Olow304/memvid/issues/49)]

* [Memary](https://kingjulio8238.github.io/memarydocs/) ❄️ Inactive (no significant development activity; last checked 2026-07)
  \[[code](https://github.com/kingjulio8238/memary) ⭐ 2,638 | 🐛 14 | 🌐 Jupyter Notebook | 📅 2024-10-22]

***

## 📖 Tutorials

#### 🗓️ 2026

* **[Agent Memory Techniques](https://github.com/NirDiamant/Agent_Memory_Techniques) ⭐ 869 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-02** (NirDiamant): 30 runnable Jupyter notebooks covering conversation buffers, vector stores, knowledge graphs, episodic and semantic memory, Mem0, MemGPT/Letta, Zep, Graphiti, and LoCoMo benchmarks
  \[[code](https://github.com/NirDiamant/Agent_Memory_Techniques) ⭐ 869 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-02]

* **[Memory, Context, and Retrieval](https://books.bloo-mind.ai/masact/ch-07-memory-context-retrieval)** †: Chapter 7 of the book *[Multi-Agent Systems: A Contemporary Treatment](https://books.bloo-mind.ai/masact/)*.

#### 🗓️ 2025

* **[ACM SIGIR-AP 2025](https://www.sigir-ap.org/sigir-ap-2025/) Tutorial: [Conversational Agents: From RAG to LTM](https://sites.google.com/view/ltm-tutorial)** †
  \[[paper](https://dl.acm.org/doi/10.1145/3767695.3769671)]
  \[[code](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory) ⭐ 581 | 🐛 1 | 🌐 Python | 📅 2026-08-13]

* Daily Dose of DS: A Practical Deep Dive Into Memory Optimization for Agentic Systems
  \[[Part-A](https://www.dailydoseofds.com/ai-agents-crash-course-part-15-with-implementation/)]
  \[[Part-B](https://www.dailydoseofds.com/ai-agents-crash-course-part-16-with-implementation/)]
  \[[Part-C](https://www.dailydoseofds.com/ai-agents-crash-course-part-17-with-implementation/)]

***

## 📚 Surveys

#### 🗓️ 2026

* **[Toward Efficient Agents: Memory, Tool Learning, and Planning](https://arxiv.org/abs/2601.14192)**
  \[[code](https://github.com/yxf203/Awesome-Efficient-Agents) ⭐ 295 | 🐛 4 | 📅 2026-08-09]

* **[Rethinking Memory Mechanisms of Foundation Agents in the Second Half: A Survey](https://arxiv.org/abs/2602.06052)**
  \[[code](https://github.com/AgentMemoryWorld/Awesome-Agent-Memory) ⭐ 196 | 🐛 5 | 📅 2026-07-23]

* [Survey on AI Memory: Theories, Taxonomies, Evaluations, and Emerging Trends](https://github.com/BAI-LAB/Survey-on-AI-Memory/blob/main/Survey%20on%20AI%20Memory.pdf) ⭐ 103 | 🐛 0 | 📅 2026-03-30

* **[From Storage to Experience: A Survey on the Evolution of LLM Agent Memory Mechanisms](https://arxiv.org/abs/2605.06716)**
  \[[code](https://github.com/FeishuLuo/Evolving-LLM-Agent-Memory-Survey) ⭐ 43 | 🐛 1 | 📅 2026-04-13]

* **[Memory in the LLM Era: Modular Architectures and Strategies within a Unified Framework](https://arxiv.org/abs/2604.01707)**
  \[[code](https://github.com/Yanchen398/Memory-in-the-LLM-Era) ⭐ 30 | 🐛 1 | 🌐 Python | 📅 2026-08-14]

* **[Anatomy of Agentic Memory: Taxonomy and Empirical Analysis of Evaluation and System Limitations](https://arxiv.org/abs/2602.19320)**
  \[[code](https://github.com/FredJiang0324/Anatomy-of-Agentic-Memory) ⭐ 25 | 🐛 0 | 📅 2026-04-08]

* [Memory for Large Language Models](https://arxiv.org/abs/2607.25380)

* [LLM Agent Memory: A Survey from a Unified Representation–Management Perspective](https://www.preprints.org/manuscript/202603.0359)

* [Memory for Autonomous LLM Agents: Mechanisms, Evaluation, and Emerging Frontiers](https://arxiv.org/abs/2603.07670)

* [Externalization in LLM Agents: A Unified Review of Memory, Skills, Protocols and Harness Engineering](https://arxiv.org/abs/2604.08224)

* [The AI Hippocampus: How Far are We From Human Memory?](https://arxiv.org/abs/2601.09113)

#### 🗓️ 2025

* **[Memory in the Age of AI Agents](https://arxiv.org/abs/2512.13564)**
  \[[code](https://github.com/Shichun-Liu/Agent-Memory-Paper-List) ⭐ 2,313 | 🐛 12 | 📅 2026-03-04]

* **[Rethinking Memory in AI: Taxonomy, Operations, Topics, and Future Directions](https://arxiv.org/abs/2505.00675)**
  \[[code](https://github.com/Elvin-Yiming-Du/Survey_Memory_in_AI) ⭐ 357 | 🐛 1 | 📅 2025-12-29]

* **[AI Meets Brain: Memory Systems from Cognitive Neuroscience to Autonomous Agents](https://arxiv.org/abs/2512.23343)**
  \[[code](https://github.com/AgentMemory/Huaman-Agent-Memory) ⭐ 114 | 🐛 0 | 📅 2025-12-30]

* [From Human Memory to AI Memory: A Survey on Memory Mechanisms in the Era of LLMs](https://arxiv.org/abs/2504.15965)

* [Cognitive Memory in Large Language Models](https://arxiv.org/abs/2504.02441)

* [Advances and Challenges in Foundation Agents: From Brain-Inspired Intelligence to Evolutionary, Collaborative, and Safe Systems (Chapter 3)](https://arxiv.org/abs/2504.01990)

* [Human-inspired Perspectives: A Survey on AI Long-term Memory](https://arxiv.org/abs/2411.00489)

#### 🗓️ 2024

* **[A Survey on the Memory Mechanism of Large Language Model based Agents](https://arxiv.org/abs/2404.13501)**
  \[[code](https://github.com/nuster1128/LLM_Agent_Memory_Survey) ⭐ 506 | 🐛 0 | 📅 2025-07-28]

***

## 📏 Benchmarks

### 💬 Plain-Text Benchmarks

#### 🗓️ 2026

* **[Agent Memory Leaderboard](https://agentmemories.ai/home)**
  \[[code](https://github.com/AML-memory/agent-memory-leaderboard) ⭐ 681 | 🐛 8 | 🌐 Python | 📅 2026-08-07]
  *Public evaluation platform: participants expose Add/Search APIs and are scored on textual-memory and coding-agent-memory tracks.*

* **[Are We Ready For An Agent-Native Memory System?](https://arxiv.org/abs/2606.24775)**
  (The MemoryData Paper)
  \[[code](https://github.com/OpenDataBox/MemoryData) ⭐ 132 | 🐛 1 | 🌐 Python | 📅 2026-07-05]

* **LoCoMo Refined: Recalibrating LoCoMo with Stricter LLM Judging and A Cleaned Dataset**
  \[[code](https://github.com/mem-eval-suite/LoCoMo_refined) ⭐ 111 | 🐛 8 | 🌐 Python | 📅 2026-05-18]

* **OmniMemEval**
  \[[code](https://github.com/MemTensor/OmniMemEval) ⭐ 43 | 🐛 1 | 🌐 Python | 📅 2026-08-13]

* **[Locomo-Plus: Beyond-Factual Cognitive Memory Evaluation Framework for LLM Agents](https://arxiv.org/abs/2602.10715)**
  \[[code](https://github.com/xjtuleeyf/Locomo-Plus) ⭐ 32 | 🐛 3 | 🌐 Python | 📅 2026-02-13]

* **[Cost and Accuracy of Long-Term Memory in Distributed Multi-Agent Systems Based on Large Language Models](https://arxiv.org/abs/2601.07978)**
  \[[code](https://github.com/wolffbe/dmas-memory) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-05-29]

* **Agent-Memory Integrity Benchmark**
  \[[code](https://github.com/DanceNitra/agent-memory-integrity) ⚠️ Archived]

#### 🗓️ 2025

* **[LongBench v2: Towards Deeper Understanding and Reasoning on Realistic Long-context Multitasks](https://arxiv.org/abs/2412.15204)**
  \[[code](https://github.com/THUDM/LongBench) ⭐ 1,219 | 🐛 67 | 🌐 Python | 📅 2025-01-15]

* **[Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions](https://arxiv.org/abs/2507.05257)**
  (The MemoryAgentBench Paper)
  \[[code](https://github.com/HUST-AI-HYZ/MemoryAgentBench) ⭐ 432 | 🐛 6 | 🌐 Python | 📅 2026-05-21]
  \[[data](https://huggingface.co/datasets/ai-hyz/MemoryAgentBench)]

* **[NoLiMa: Long-Context Evaluation Beyond Literal Matching](https://arxiv.org/abs/2502.05167)**
  \[[code](https://github.com/adobe-research/NoLiMa) ⭐ 201 | 🐛 6 | 🌐 Python | 📅 2025-07-17]
  \[[data](https://github.com/adobe-research/NoLiMa/tree/main/data) ⭐ 201 | 🐛 6 | 🌐 Python | 📅 2025-07-17]

* **[Know Me, Respond to Me: Benchmarking LLMs for Dynamic User Profiling and Personalized Responses at Scale](https://arxiv.org/abs/2504.14225)**
  (The PersonaMem and ImplicitPersona Paper)
  \[[code](https://github.com/bowen-upenn/PersonaMem) ⭐ 187 | 🐛 7 | 🌐 Python | 📅 2026-03-19]
  \[[data11](https://huggingface.co/datasets/bowen-upenn/PersonaMem)]
  \[[data2](https://huggingface.co/datasets/bowen-upenn/ImplicitPersona)]

* **[HaluMem: Evaluating Hallucinations in Memory Systems of Agents](http://arxiv.org/abs/2511.03506)**
  \[[code](https://github.com/MemTensor/HaluMem) ⭐ 152 | 🐛 0 | 🌐 Python | 📅 2026-04-30]
  \[[data](https://huggingface.co/datasets/IAAR-Shanghai/HaluMem)]

* **[Beyond a Million Tokens: Benchmarking and Enhancing Long-Term Memory in LLMs](https://arxiv.org/abs/2510.27246)**
  (The BEAM Paper)
  \[[code](https://github.com/mohammadtavakoli78/BEAM) ⭐ 121 | 🐛 10 | 🌐 Python | 📅 2026-02-02]
  \[[data](https://huggingface.co/datasets/Mohammadta/BEAM)]

* **[LifelongAgentBench: Evaluating LLM Agents as Lifelong Learners](https://arxiv.org/abs/2505.11942)**
  \[[code](https://github.com/caixd-220529/LifelongAgentBench) ⭐ 96 | 🐛 1 | 🌐 Python | 📅 2025-05-30]
  \[[data](https://huggingface.co/datasets/csyq/LifelongAgentBench)]

* **[MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents](https://arxiv.org/abs/2506.21605)**
  \[[code](https://github.com/import-myself/Membench) ⭐ 57 | 🐛 1 | 🌐 Python | 📅 2025-11-27]

* **[MOOM: Maintenance, Organization and Optimization of Memory in Ultra-Long Role-Playing Dialogues](https://arxiv.org/abs/2509.11860)**
  (The ZH-4O Paper)
  \[[code](https://github.com/cows21/MOOM-Roleplay-Dialogue) ⭐ 13 | 🐛 0 | 🌐 Python | 📅 2025-05-19]
  \[[data](https://github.com/cows21/MOOM-Roleplay-Dialogue/tree/main/data) ⭐ 13 | 🐛 0 | 🌐 Python | 📅 2025-05-19]

* **[Minerva: A Programmable Memory Test Benchmark for Language Models](https://arxiv.org/abs/2502.03358)**
  \[[code](https://github.com/microsoft/minerva_memory_test) ⚠️ Archived]

* [Evo-Memory: Benchmarking LLM Agent Test-time Learning with Self-Evolving Memory](https://arxiv.org/abs/2511.20857)

* [OdysseyBench: Evaluating LLM Agents on Long-Horizon Complex Office Application Workflows](https://arxiv.org/abs/2508.09124)

#### 🗓️ 2024

* **[LongBench: A Bilingual, Multitask Benchmark for Long Context Understanding](https://arxiv.org/abs/2308.14508)**
  \[[code](https://github.com/THUDM/LongBench) ⭐ 1,219 | 🐛 67 | 🌐 Python | 📅 2025-01-15]

* **[Evaluating Very Long-Term Conversational Memory of LLM Agents](https://arxiv.org/abs/2402.17753)**
  (The LoCoMo Paper)
  \[[code](https://github.com/snap-research/LoCoMo) ⭐ 1,096 | 🐛 37 | 🌐 Python | 📅 2024-08-13]
  \[[data](https://github.com/snap-research/locomo/tree/main/data) ⭐ 1,096 | 🐛 37 | 🌐 Python | 📅 2024-08-13]

* **[LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory](https://arxiv.org/abs/2410.10813)**
  \[[data](https://github.com/xiaowu0162/LongMemEval) ⭐ 1,001 | 🐛 43 | 🌐 Python | 📅 2026-05-11]

* **[∞Bench: Extending Long Context Evaluation Beyond 100K Tokens](https://arxiv.org/abs/2402.13718v3)**
  \[[code](https://github.com/OpenBMB/InfiniteBench) ⭐ 389 | 🐛 10 | 🌐 Python | 📅 2024-09-25]

#### 🗓️ 2023

* **[StoryBench: A Multifaceted Benchmark for Continuous Story Visualization](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f63f5fbed1a4ef08c857c5f377b5d33a-Abstract-Datasets_and_Benchmarks.html)**
  \[[code](https://github.com/google/storybench) ⚠️ Archived]

### 🎬 Multimodal Benchmarks

#### 🗓️ 2026

* **[RMBench: Memory-Dependent Robotic Manipulation Benchmark with Insights into Policy Design](https://arxiv.org/abs/2603.01229)**
  \[[code](https://github.com/robotwin-Platform/rmbench) ⭐ 196 | 🐛 13 | 🌐 Python | 📅 2026-07-14]
  \[[proj](https://rmbench.github.io/)]

* **[RoboMemArena: A Comprehensive and Challenging Robotic Memory Benchmark](https://arxiv.org/abs/2605.10921)**
  \[[code](https://github.com/OpenHelix-Team/RoboMemArena) ⭐ 192 | 🐛 7 | 🌐 Python | 📅 2026-08-07]
  \[[data](https://huggingface.co/datasets/RoboMemArenaBenchmark/RoboMemArena)]
  \[[proj](https://robomemarena.github.io/)]
  \[[leaderboard](https://robomemarena.github.io/leaderboard.html)]

* **[Persona-MME: A Benchmark for Long-Term Personalized Multimodal LLMs](https://arxiv.org/abs/2604.13074)**
  \[[code](https://github.com/MiG-NJU/PersonaVLM) ⭐ 115 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-04-16]
  \[[data](https://huggingface.co/datasets/ClareNie/Persona-MME)]

* **[MBench: A Comprehensive Benchmark on Memory Capability for Video World Models](https://arxiv.org/abs/2606.00793)**
  \[[code](https://github.com/study-overflow/MBench) ⭐ 114 | 🐛 2 | 🌐 Python | 📅 2026-06-02]
  \[[proj](https://peanutup.github.io/MBench-project/)]
  \[[leaderboard](https://huggingface.co/spaces/study-overflow/MBench_Leaderboard)]

* **[DeepImageSearch: Benchmarking Multimodal Agents for Context-Aware Image Retrieval in Visual Histories](https://arxiv.org/abs/2602.10809)**
  \[[code](https://github.com/RUC-NLPIR/DeepImageSearch) ⭐ 87 | 🐛 0 | 🌐 Python | 📅 2026-05-02]
  \[[data](https://huggingface.co/datasets/RUC-NLPIR/DISBench)]
  \[[leaderboard](https://huggingface.co/spaces/RUC-NLPIR/DISBench-Leaderboard)]

#### 🗓️ 2025

* **[Video-MME: The First-Ever Comprehensive Evaluation Benchmark of Multi-modal LLMs in Video Analysis](https://arxiv.org/abs/2405.21075v3)**
  \[[code](https://github.com/MME-Benchmarks/Video-MME) ⭐ 789 | 🐛 11 | 📅 2025-12-08]

* **[LVBench: An Extreme Long Video Understanding Benchmark](https://arxiv.org/abs/2406.08035)**
  \[[code](https://github.com/zai-org/LVBench) ⭐ 144 | 🐛 12 | 🌐 Python | 📅 2025-07-09]

* **[TeleEgo: Benchmarking Egocentric AI Assistants in the Wild](https://arxiv.org/abs/2510.23981)** †
  \[[code](https://github.com/TeleAI-UAGI/TeleEgo) ⭐ 64 | 🐛 0 | 🌐 Python | 📅 2026-08-10]
  \[[data](https://huggingface.co/datasets/David0219/TeleEgo)]
  \[[proj](https://programmergg.github.io/jrliu.github.io/)]
  \[[leaderboard](https://programmergg.github.io/jrliu.github.io/#leaderboard)]

#### 🗓️ 2024

* **[MovieChat+: Question-aware Sparse Memory for Long Video Question Answering](https://arxiv.org/abs/2404.17176)**
  \[[code](https://github.com/rese1f/MovieChat) ⭐ 706 | 🐛 42 | 🌐 Python | 📅 2025-01-29]

* **[LongVideoBench: A Benchmark for Long-Context Interleaved Video-Language Understanding](https://arxiv.org/abs/2407.15754)**
  \[[code](https://github.com/longvideobench/LongVideoBench) ⭐ 136 | 🐛 12 | 🌐 Python | 📅 2024-07-27]

* **[CinePile: A Long Video Question Answering Dataset and Benchmark](https://arxiv.org/abs/2405.08813)**
  \[[code](https://huggingface.co/datasets/tomg-group-umd/cinepile)]

#### 🗓️ 2023

* **[EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding](https://proceedings.neurips.cc/paper_files/paper/2023/file/90ce332aff156b910b002ce4e6880dec-Paper-Datasets_and_Benchmarks.pdf)**
  \[[code](https://github.com/egoschema/egoschema) ⭐ 117 | 🐛 5 | 🌐 Python | 📅 2024-12-30]

* [LvBench: A Benchmark for Long-form Video Understanding with Versatile Multi-modal Question Answering](https://arxiv.org/abs/2312.04817)

### 🎮 Dynamic Benchmarks & Simulation Environments

#### 🗓️ 2026

* **[AMemGym: Interactive Memory Benchmarking for Assistants in Long-Horizon Conversations](https://arxiv.org/abs/2603.01966)**
  \[[code](https://github.com/AGI-Eval-Official/amemgym) ⭐ 42 | 🐛 2 | 🌐 Python | 📅 2026-04-07]
  \[[proj](https://agi-eval-official.github.io/amemgym/)]

* **[SEAGym: An Evaluation Environment for Self-Evolving LLM Agents](https://arxiv.org/abs/2606.17546)**
  \[[code](https://github.com/antropy-research/SEAGym) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-07-13]

* **[Beyond Static Dialogues: Benchmarking Realistic, Heterogeneous, and Evolving Long-Term Memory](https://arxiv.org/abs/2605.31086)**
  \[[code](https://github.com/microsoft/RHELM) ⭐ 12 | 🐛 0 | 🌐 HTML | 📅 2026-06-05]
  \[[data](https://huggingface.co/datasets/microsoft/RHELM)]
  \[[proj](https://microsoft.github.io/RHELM/)]

* [StreamMemBench: Streaming Evaluation of Agent Memory for Future-Oriented Assistance](https://arxiv.org/abs/2606.14571)

#### 🗓️ 2025

* **[ARE: Scaling Up Agent Environments and Evaluations](https://arxiv.org/abs/2509.17158)**
  (The Gaia2 Paper)
  \[[code](https://github.com/facebookresearch/meta-agents-research-environments) ⭐ 543 | 🐛 38 | 🌐 Python | 📅 2026-08-11]

* **[MemoryBench: A Benchmark for Memory and Continual Learning in LLM Systems](https://arxiv.org/abs/2510.17281)**
  \[[code](https://github.com/LittleDinoC/MemoryBench) ⭐ 89 | 🐛 1 | 🌐 Python | 📅 2026-06-27]
  \[[data](https://huggingface.co/datasets/THUIR/MemoryBench)]

#### 🗓️ 2024

* **[AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents](https://arxiv.org/abs/2407.18901)**
  \[[code](https://github.com/StonyBrookNLP/appworld) ⭐ 483 | 🐛 8 | 🌐 Python | 📅 2026-02-17]

***

## 🔤 Papers - Nonparametric Memory

### 📝 Text Memory

#### 🗓️ 2026

* **[SimpleMem: Efficient Lifelong Memory for LLM Agents](https://arxiv.org/abs/2601.02553)**
  \[[code](https://github.com/aiming-lab/SimpleMem) ⭐ 3,702 | 🐛 3 | 🌐 Python | 📅 2026-07-24]

* **[AutoMem: Automated Learning of Memory as a Cognitive Skill](https://arxiv.org/abs/2607.01224)**
  \[[code](https://github.com/autoLearnMem/AutoMem) ⭐ 135 | 🐛 1 | 🌐 Python | 📅 2026-07-03]
  \[[proj](https://autolearnmem.github.io/)]

* **[MemPrivacy: Privacy-Preserving Personalized Memory Management for Edge-Cloud Agents](https://arxiv.org/abs/2605.09530)**
  \[[code](https://github.com/MemTensor/MemPrivacy) ⭐ 120 | 🐛 0 | 🌐 Python | 📅 2026-06-16]

* **[Beyond RAG for Agent Memory: Retrieval by Decoupling and Aggregation](https://arxiv.org/abs/2602.02007)**
  \[[code](https://github.com/HU-xiaobai/xMemory) ⭐ 119 | 🐛 2 | 🌐 Python | 📅 2026-02-25]

* **[Mandol: An Agglomerative Agent Memory System for Long-Term Conversations](https://arxiv.org/abs/2606.29778)**
  \[[code](https://github.com/AgentCombo/Mandol) ⭐ 54 | 🐛 0 | 🌐 Python | 📅 2026-08-02]

* **[Beyond Similarity Search: Tenure and the Case for Structured Belief State in LLM Memory](https://arxiv.org/abs/2605.11325)**
  \[[code](https://github.com/jeffreyflynt/tenure) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-07-17]

* **[RecMem: Recurrence-based Memory Consolidation for Efficient and Effective Long-Running LLM Agents](https://arxiv.org/abs/2605.16045)**
  \[[code](https://github.com/CaiusDai/RecMem) ⭐ 13 | 🐛 0 | 🌐 Python | 📅 2026-05-15]

* **[Evoking User Memory: Personalizing LLM via Recollection-Familiarity Adaptive Retrieval](https://arxiv.org/abs/2603.09250)** (RF-Mem)
  \[[code](https://github.com/Applied-Machine-Learning-Lab/ICLR2026_RF-Mem) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2026-02-25]

* **[MemSearch-o1: Empowering Large Language Models with Reasoning-Aligned Memory Growth in Agentic Search](https://arxiv.org/abs/2604.17265)**
  \[[code](https://github.com/Applied-Machine-Learning-Lab/ACL2026_MemSearch-o1) ⭐ 4 | 🐛 0 | 📅 2025-10-07]

* **[Memory Efficiency and Resource-Rational Encoding in Sentence Processing](https://aclanthology.org/2026.acl-long.1550/)**
  \[[code](https://github.com/weijiexu-charlie/resource-rational-encoding) ⭐ 2 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-04-13]

* [MemCompiler: Compile, Don't Inject -- State-Conditioned Memory for Embodied Agents](https://arxiv.org/abs/2605.07594)

#### 🗓️ 2025

* **[LightMem: Lightweight and Efficient Memory-Augmented Generation](https://arxiv.org/abs/2510.18866)**
  \[[code](https://github.com/zjunlp/LightMem) ⭐ 1,084 | 🐛 3 | 🌐 Python | 📅 2026-08-06]

* **[Human-inspired Episodic Memory for Infinite Context LLMs](https://arxiv.org/abs/2407.09450)**
  \[[code](https://github.com/em-llm/EM-LLM-model) ⭐ 282 | 🐛 5 | 🌐 Python | 📅 2025-03-06]

* **[What Deserves Memory: Adaptive Memory Distillation for LLM Agents](https://arxiv.org/abs/2508.03341)**
  \[[code](https://github.com/nemori-ai/nemori) ⭐ 209 | 🐛 6 | 🌐 Python | 📅 2026-04-16]

* **[MemWeaver: A Hierarchical Memory from Textual Interactive Behaviors for Personalized Generation](https://arxiv.org/abs/2510.07713)**
  \[[code](https://github.com/fishsure/MemWeaver) ⭐ 14 | 🐛 3 | 🌐 Python | 📅 2026-05-18]

* [Evaluating Long-Term Memory for Long-Context Question Answering](https://arxiv.org/abs/2510.23730)

* [Text2Mem: A Unified Memory Operation Language for Memory Operating System](https://arxiv.org/abs/2509.11145)

* [O-Mem: Omni Memory System for Personalized, Long Horizon, Self-Evolving Agents](https://arxiv.org/abs/2511.13593)

* [Omne-R1: Learning to Reason with Memory for Multi-hop Question Answering](https://arxiv.org/abs/2508.17330)

* [In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents](https://aclanthology.org/2025.acl-long.413/)

* [SEDM: Scalable Self-Evolving Distributed Memory for Agents](https://arxiv.org/abs/2509.09498)

* [MemoRAG: Boosting Long Context Processing with Global Memory-Enhanced Retrieval Augmentation](https://arxiv.org/abs/2409.05591)

* [Towards LifeSpan Cognitive Systems](https://arxiv.org/abs/2409.13265)

#### 🗓️ 2024

* **[Agent Workflow Memory](https://arxiv.org/abs/2409.07429)**
  \[[code](https://github.com/zorazrw/agent-workflow-memory) ⭐ 458 | 🐛 4 | 🌐 Python | 📅 2025-12-22]

* **[MemoryBank: Enhancing Large Language Models with Long-Term Memory](https://arxiv.org/abs/2305.10250)**
  \[[code](https://github.com/zhongwanjun/MemoryBank-SiliconFriend) ⭐ 444 | 🐛 16 | 🌐 Python | 📅 2023-05-24]

* **[Compress to Impress: Unleashing the Potential of Compressive Memory in Real-World Long-Term Conversations](https://arxiv.org/abs/2402.11975)**
  \[[code](https://github.com/nuochenpku/COMEDY) ⭐ 25 | 🐛 0 | 🌐 Python | 📅 2024-11-18]

* **[Toward Conversational Agents with Context and Time Sensitive Long-term Memory](https://arxiv.org/abs/2406.00057)**
  \[[data](https://github.com/Zyphra/TemporalMemoryDataset) ⭐ 13 | 🐛 0 | 📅 2024-06-04]

* [InfLLM: Training-Free Long-Context Extrapolation for LLMs with an Efficient Context Memory](https://arxiv.org/abs/2402.04617)

#### 🗓️ 2023

* [RET-LLM: Towards a General Read-Write Memory for Large Language Models](https://arxiv.org/abs/2305.14322)

### 🌐 Graph Memory

#### 🗓️ 2026

* **[HyperMem: Hypergraph Memory for Long-Term Conversations](https://arxiv.org/abs/2604.08256)**
  \[[code](https://github.com/EverMind-AI/EverOS) ⭐ 12,005 | 🐛 71 | 🌐 Python | 📅 2026-08-13]

* **[Rethinking Memory as Continuously Evolving Connectivity](https://arxiv.org/abs/2605.28773)** (FluxMem)
  \[[code](https://github.com/zjunlp/LightMem) ⭐ 1,084 | 🐛 3 | 🌐 Python | 📅 2026-08-06]

* **[PlugMem: A Task-Agnostic Plugin Memory Module for LLM Agents](https://arxiv.org/abs/2603.03296)**
  \[[code](https://github.com/TIMAN-group/PlugMem) ⭐ 286 | 🐛 5 | 🌐 Python | 📅 2026-07-09]

* **[MAGMA: A Multi-Graph based Agentic Memory Architecture for AI Agents](https://arxiv.org/abs/2601.03236)**
  \[[code](https://github.com/FredJiang0324/MAMGA) ⭐ 154 | 🐛 0 | 🌐 Python | 📅 2026-07-10]

* **[Mnemis: Dual-Route Retrieval on Hierarchical Graphs for Long-Term LLM Memory](https://arxiv.org/abs/2602.15313)**
  \[[code](https://github.com/microsoft/Mnemis) ⭐ 104 | 🐛 0 | 🌐 Python | 📅 2026-04-14]

* **[TraceMem: Weaving Narrative Memory Schemata from User Conversational Traces](https://arxiv.org/abs/2602.09712)**
  \[[code](https://github.com/YimingShu-teay/TraceMem) ⭐ 48 | 🐛 0 | 🌐 Python | 📅 2026-02-19]

* **[GraphPlanner: Graph Memory-Augmented Agentic Routing for Multi-Agent LLMs](https://arxiv.org/abs/2604.23626)**
  \[[code](https://github.com/ulab-uiuc/GraphPlanner) ⭐ 15 | 🐛 1 | 🌐 Python | 📅 2026-04-26]

* [SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory](https://arxiv.org/abs/2605.12061)

#### 🗓️ 2025

* **[From RAG to Memory: Non-Parametric Continual Learning for Large Language Models](https://arxiv.org/abs/2502.14802)**
  \[[code](https://github.com/OSU-NLP-Group/HippoRAG) ⭐ 3,940 | 🐛 7 | 🌐 Python | 📅 2026-07-29]

* **[MIRIX: Multi-Agent Memory System for LLM-Based Agents](https://arxiv.org/abs/2507.07957)**
  \[[code](https://github.com/Mirix-AI/MIRIX) ⭐ 3,482 | 🐛 44 | 🌐 Python | 📅 2026-08-11]

* **[From Single to Multi-Granularity: Toward Long-Term Memory Association and Selection of Conversational Agents](https://arxiv.org/abs/2505.19549)** (MemGAS)
  \[[code](https://github.com/quqxui/MemGAS) ⭐ 18 | 🐛 1 | 🌐 Python | 📅 2026-03-15]

* **[Hierarchical Memory Organization for Wikipedia Generation](https://aclanthology.org/2025.acl-long.1423/)**
  \[[code](https://github.com/eugeneyujunhao/mog) ⭐ 0 | 🐛 0 | 📅 2025-06-29]

* [From Experience to Strategy: Empowering LLM Agents with Trainable Graph Memory](https://www.arxiv.org/abs/2511.07800)

* [Bridging Intuitive Associations and Deliberate Recall: Empowering LLM Personal Assistant with Graph-Structured Long-term Memory](https://aclanthology.org/2025.findings-acl.901/)

* [HiAgent: Hierarchical Working Memory Management for Solving Long-Horizon Agent Tasks with Large Language Model](https://aclanthology.org/2025.acl-long.1575/)

* [Optimizing the Interface Between Knowledge Graphs and LLMs for Complex Reasoning](https://arxiv.org/abs/2505.24478)

#### 🗓️ 2024

* **[HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models](https://arxiv.org/abs/2405.14831)**
  \[[code](https://github.com/OSU-NLP-Group/HippoRAG) ⭐ 3,940 | 🐛 7 | 🌐 Python | 📅 2026-07-29]

* **[AriGraph: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents](https://arxiv.org/abs/2407.04363)**
  \[[code](https://github.com/AIRI-Institute/AriGraph) ⭐ 173 | 🐛 2 | 🌐 Inform 7 | 📅 2024-09-10]

### 🎥 Multimodal Memory (for Understanding)

#### 🗓️ 2026

* **[Omni-SimpleMem: Autoresearch-Guided Discovery of Lifelong Multimodal Agent Memory](https://arxiv.org/abs/2604.01007)**
  \[[code](https://github.com/aiming-lab/SimpleMem) ⭐ 3,702 | 🐛 3 | 🌐 Python | 📅 2026-07-24]

* **[PersonaVLM: Long-Term Personalized Multimodal LLMs](https://arxiv.org/abs/2604.13074)**
  \[[code](https://github.com/MiG-NJU/PersonaVLM) ⭐ 115 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-04-16]
  \[[proj](https://PersonaVLM.github.io)]

* **[HERMES: KV Cache as Hierarchical Memory for Efficient Streaming Video Understanding](https://arxiv.org/abs/2601.14724)**
  \[[code](https://github.com/haowei-freesky/HERMES) ⭐ 94 | 🐛 1 | 🌐 Python | 📅 2026-05-08]

* **[MemGUI-Agent: An End-to-End Long-Horizon Mobile GUI Agent with Proactive Context Management](https://arxiv.org/abs/2606.19926)**
  \[[code](https://github.com/kwai/MemGUI-Agent) ⭐ 88 | 🐛 1 | 🌐 Python | 📅 2026-07-08]
  \[[proj](https://memgui-agent.github.io/)]

* **[FluxMem: Adaptive Hierarchical Memory for Streaming Video Understanding](https://arxiv.org/abs/2603.02096)**
  \[[code](https://github.com/YiwengXie/FluxMem) ⭐ 76 | 🐛 3 | 🌐 Python | 📅 2026-03-16]
  \[[proj](https://yiwengxie.com/FluxMem/)]

* **[SE-GA: Memory-Augmented Self-Evolution for GUI Agents](https://arxiv.org/abs/2605.16883)**
  \[[code](https://github.com/jinshilong-dev/SE-GA) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-06-02]

* **[Visual Agentic Memory: Enabling Online Long Video Understanding via Online Indexing, Hierarchical Memory, and Agentic Retrieval](https://arxiv.org/abs/2605.16481)**
  \[[code](https://github.com/yiliu-li/Visual-Agentic-Memory) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-08-07]

* **[EventMemAgent: Hierarchical Event-Centric Memory for Online Video Understanding with Adaptive Tool Use](https://arxiv.org/abs/2602.15329)**
  \[[code](https://github.com/lingcco/EventMemAgent) ⭐ 8 | 🐛 4 | 📅 2026-02-20]

* **[M2A: Multimodal Memory Agent with Dual-Layer Hybrid Memory for Long-Term Personalized Interactions](https://arxiv.org/abs/2602.07624)**
  \[[code](https://github.com/Little-Fridge/M2A) ⭐ 8 | 🐛 2 | 🌐 Python | 📅 2026-02-20]

* [NativeMEM: Native Memory Compression for Long-Horizon Robotic Manipulation](https://arxiv.org/abs/2607.06678)
  \[[proj](https://opendrivelab.com/NativeMEM/)]

#### 🗓️ 2025

* **[Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory](https://arxiv.org/abs/2508.09736)**
  \[[code](https://github.com/bytedance-seed/m3-agent) ⭐ 1,441 | 🐛 18 | 🌐 Python | 📅 2026-02-12]

* **[MemVerse: Multimodal Memory for Lifelong Learning Agents](https://arxiv.org/abs/2512.03627)**
  \[[code](https://github.com/KnowledgeXLab/MemVerse) ⭐ 154 | 🐛 0 | 🌐 Python | 📅 2026-03-17]

* **[WorldMM: Dynamic Multimodal Memory Agent for Long Video Reasoning](https://arxiv.org/abs/2512.02425)**
  \[[code](https://github.com/wgcyeo/WorldMM) ⭐ 103 | 🐛 1 | 🌐 Python | 📅 2026-07-29]

* **[HippoMM: Hippocampal-inspired Multimodal Memory for Long Audiovisual Event Understanding](https://arxiv.org/abs/2504.10739)**
  \[[code](https://github.com/linyueqian/HippoMM) ⭐ 22 | 🐛 0 | 🌐 Python | 📅 2025-05-22]

* **[MGA: Memory-Driven GUI Agent for Observation-Centric Interaction](https://arxiv.org/abs/2510.24168)**
  \[[code](https://github.com/MintyCo0kie/MGA4OSWorld) ⭐ 8 | 🐛 0 | 🌐 Python | 📅 2026-04-13]

* [Infinite Video Understanding](https://www.arxiv.org/abs/2507.09068)

* [Episodic Memory Representation for Long-form Video Understanding](https://arxiv.org/abs/2508.09486)

* [Multi-RAG: A Multimodal Retrieval-Augmented Generation System for Adaptive Video Understanding](https://arxiv.org/abs/2505.23990)

* [Contextual Experience Replay for Self-Improvement of Language Agents](https://arxiv.org/abs/2506.06698)

#### 🗓️ 2024

* **[VideoAgent: Long-form Video Understanding with Large Language Model as Agent](https://arxiv.org/abs/2403.10517)**
  \[[code](https://github.com/HKUDS/VideoAgent) ⭐ 1,713 | 🐛 13 | 🌐 Python | 📅 2026-07-22]

* **[VideoChat-Flash: Hierarchical Compression for Long-Context Video Modeling](https://arxiv.org/abs/2501.00574)**
  \[[code](https://github.com/OpenGVLab/VideoChat-Flash) ⭐ 527 | 🐛 10 | 🌐 Python | 📅 2026-07-19]

* **[LongVLM: Efficient Long Video Understanding via Large Language Models](https://arxiv.org/abs/2404.03384)**
  \[[code](https://github.com/ziplab/LongVLM) ⭐ 108 | 🐛 10 | 🌐 Python | 📅 2024-07-30]

* **[KARMA: Augmenting Embodied AI Agents with Long-and-short Term Memory Systems](https://arxiv.org/abs/2409.14908)**
  \[[code](https://github.com/WZX0Swarm0Robotics/KARMA/tree/master) ⭐ 11 | 🐛 0 | 📅 2025-03-20]

### 🎥 Multimodal Memory (for Generation)

#### 🗓️ 2026

* **[MemSlides: A Hierarchical Memory Driven Agent Framework for Personalized Slide Generation with Multi-turn Local Revision](https://arxiv.org/abs/2606.17162)**
  \[[code](https://github.com/huohua325/Memslides) ⭐ 1,083 | 🐛 3 | 🌐 Python | 📅 2026-08-06]
  \[[proj](https://memslides.github.io/)]

* **[LoGeR: Long-Context Geometric Reconstruction with Hybrid Memory](https://arxiv.org/abs/2603.03269)**
  \[[code](https://github.com/Junyi42/LoGeR) ⭐ 611 | 🐛 6 | 🌐 Python | 📅 2026-04-27]

* [OneStory: Coherent Multi-Shot Video Generation with Adaptive Memory](https://arxiv.org/abs/2512.07802)

#### 🗓️ 2025

* **[StoryMem: Multi-shot Long Video Storytelling with Memory](https://arxiv.org/abs/2512.19539)**
  \[[code](https://github.com/Kevin-thu/StoryMem) ⭐ 761 | 🐛 7 | 🌐 Python | 📅 2026-07-22]

* **[Yume-1.5: A Text-Controlled Interactive World Generation Model](https://arxiv.org/abs/2512.22096)**
  \[[code](https://github.com/stdstu12/YUME) ⭐ 683 | 🐛 18 | 🌐 Python | 📅 2026-01-14]

* **[MemFlow: Flowing Adaptive Memory for Consistent and Efficient Long Video Narratives](https://arxiv.org/abs/2512.14699)**
  \[[code](https://github.com/KlingTeam/MemFlow) ⭐ 216 | 🐛 4 | 🌐 Python | 📅 2025-12-29]

* **[VideoRAG: Retrieval-Augmented Generation over Video Corpus](http://arxiv.org/abs/2501.05874)**
  \[[code](https://github.com/starsuzi/VideoRAG) ⭐ 84 | 🐛 5 | 🌐 Python | 📅 2025-03-17]

* **[MagicWorld: Towards Long-Horizon Stability for Interactive Video World Exploration](https://arxiv.org/abs/2511.18886)**
  \[[code](https://github.com/vivoCameraResearch/Magic-World) ⭐ 66 | 🐛 0 | 🌐 Python | 📅 2026-04-11]

* **[MotionRAG: Motion Retrieval-Augmented Image-to-Video Generation](http://arxiv.org/abs/2509.26391)**
  \[[code](https://github.com/MCG-NJU/MotionRAG) ⭐ 27 | 🐛 2 | 🌐 Python | 📅 2025-10-09]

* [Pretraining Frame Preservation in Autoregressive Video Memory Compression](https://arxiv.org/abs/2512.23851)

* [EgoLCD: Egocentric Video Generation with Long Context Diffusion](https://arxiv.org/abs/2512.04515)

* [Pack and Force Your Memory: Long-form and Consistent Video Generation](http://arxiv.org/abs/2510.01784)

* [Video World Models with Long-term Spatial Memory](http://arxiv.org/abs/2506.05284)

* [Mixture of Contexts for Long Video Generation](http://arxiv.org/abs/2508.21058)

* [Context as Memory: Scene-Consistent Interactive Long Video Generation with Memory Retrieval](http://arxiv.org/abs/2506.03141)

## 🔢 Papers - Parametric Memory

#### 🗓️ 2026

* **[Conditional Memory via Scalable Lookup: A New Axis of Sparsity for Large Language Models](https://arxiv.org/abs/2601.07372)**
  (The DeepSeek **Engram** Paper)
  \[[code](https://github.com/deepseek-ai/Engram/) ⭐ 4,589 | 🐛 20 | 🌐 Python | 📅 2026-01-14]
  * **[Beyond Conditional Computation: Retrieval-Augmented Genomic Foundation Models with Gengram](https://arxiv.org/abs/2601.22203)**
    \[[code](https://github.com/zhejianglab/Gengram/) ⭐ 50 | 🐛 0 | 🌐 Python | 📅 2026-03-17]
  * [Pooling Engram Conditional Memory in Large Language Models using CXL](https://arxiv.org/abs/2603.10087)
  * [A Collision-Free Hot-Tier Extension for Engram-Style Conditional Memory: A Controlled Study of Training Dynamics](https://arxiv.org/abs/2601.16531)

* **[MSA: Memory Sparse Attention for Efficient End-to-End Memory Model Scaling to 100M Tokens](https://github.com/EverMind-AI/MSA/blob/main/paper/MSA__Memory_Sparse_Attention_for_Efficient_End_to_End_Memory_Model_Scaling_to_100M_Tokens.pdf) ⭐ 3,513 | 🐛 4 | 🌐 Python | 📅 2026-05-06**
  \[[code](https://github.com/EverMind-AI/MSA) ⭐ 3,513 | 🐛 4 | 🌐 Python | 📅 2026-05-06]

* **[STEM: Scaling Transformers with Embedding Modules](https://arxiv.org/abs/2601.10639)**
  \[[code](https://github.com/Infini-AI-Lab/STEM) ⭐ 66 | 🐛 3 | 🌐 Python | 📅 2026-05-07]

* **[δ-mem: Efficient Online Memory for Large Language Models](https://arxiv.org/abs/2605.12357)**
  \[[code](https://github.com/MindLab-Research/delta-Mem) ⭐ 52 | 🐛 1 | 🌐 Python | 📅 2026-05-27]

* **[MeMo: Memory as a Model](https://arxiv.org/abs/2605.15156)**
  \[[code](https://github.com/arunv3rma/MeMo) ⭐ 50 | 🐛 0 | 🌐 Python | 📅 2026-05-21]

* **[GradMem: Learning to Write Context into Memory with Test-Time Gradient Descent](https://arxiv.org/abs/2603.13875)**
  \[[code](https://github.com/yurakuratov/gradmem) ⭐ 39 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2026-08-06]

* **[MeKi: Memory-based Expert Knowledge Injection for Efficient LLM Scaling](https://arxiv.org/abs/2602.03359)**
  \[[code](https://github.com/ningding-o/MeKi) ⭐ 29 | 🐛 1 | 🌐 Python | 📅 2026-03-05]

* **[Language Model Memory and Memory Models for Language](https://arxiv.org/abs/2602.13466)**
  \[[code](https://github.com/blbadger/memorymodels) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-06-10]

* [Language Models Need Sleep: Learning to Self-Modify and Consolidate Memories](https://arxiv.org/abs/2606.03979)

* [Do Language Models Need Sleep? Offline Recurrence for Improved Online Inference](https://arxiv.org/abs/2605.26099)

* [Training Transformers for KV Cache Compressibility](https://arxiv.org/abs/2605.05971)

* [Contextual Agentic Memory is a Memo, Not True Memory](https://arxiv.org/abs/2604.27707)

* [Memory Caching: RNNs with Growing Memory](https://arxiv.org/abs/2602.24281)

* [Fast-weight Product Key Memory](https://arxiv.org/abs/2601.00671)

#### 🗓️ 2025

* **[MoM: Linear Sequence Modeling with Mixture-of-Memories](https://arxiv.org/abs/2502.13685)**
  \[[code](https://github.com/OpenSparseLLMs/MoM) ⭐ 139 | 🐛 2 | 🌐 Python | 📅 2026-02-04]

* **[Memory Decoder: A Pretrained, Plug-and-Play Memory for Large Language Models](https://www.arxiv.org/abs/2508.09874)**
  \[[code](https://github.com/LUMIA-Group/MemoryDecoder) ⭐ 78 | 🐛 2 | 🌐 Python | 📅 2025-09-29]

* **[MLP Memory: Language Modeling with Retriever-pretrained External Memory](https://arxiv.org/abs/2508.01832)**
  \[[code](https://github.com/Rubin-Wei/MLPMemory) ⭐ 71 | 🐛 0 | 🌐 Python | 📅 2026-06-11]

* **[Little By Little: Continual Learning via Incremental Mixture of Rank-1 Associative Memory Experts](https://arxiv.org/abs/2506.21035)**
  \[[code](https://github.com/Artificer-AI-Lab/MoRAM) ⭐ 8 | 🐛 0 | 🌐 Python | 📅 2026-06-23]
  \[[proj](https://artificer-ai-lab.github.io/MoRAM/)]

* [How Much Do Language Models Memorize?](https://arxiv.org/abs/2505.24832)

* [Memory Retrieval and Consolidation in Large Language Models through Function Tokens](https://arxiv.org/abs/2510.08203)

* [Nested Learning: The Illusion of Deep Learning Architectures](https://openreview.net/forum?id=nbMeRvNb7A)

* [Improving Factuality with Explicit Working Memory](https://arxiv.org/abs/2412.18069)

* [R<sup>3</sup>Mem: Bridging Memory Retention and Retrieval via Reversible Compression](https://arxiv.org/abs/2502.15957)

* [May the Memory Be With You: Efficient and Infinitely Updatable State for Large Language Models](https://dl.acm.org/doi/abs/10.1145/3721146.3721951)

* [MeMo: Towards Language Models with Associative Memory Mechanisms](https://aclanthology.org/2025.findings-acl.785/)

* [REFRAG: Rethinking RAG based Decoding](https://arxiv.org/abs/2509.01092)

* [EpMAN: Episodic Memory AttentioN for Generalizing to Longer Contexts](https://aclanthology.org/2025.acl-long.574/)

* [Disentangling Memory and Reasoning Ability in Large Language Models](https://aclanthology.org/2025.acl-long.84/)

#### 🗓️ 2024

* **[WISE: Rethinking the Knowledge Memory for Lifelong Model Editing of Large Language Models](https://arxiv.org/abs/2405.14768)**
  \[[code](https://github.com/zjunlp/EasyEdit) ⭐ 2,897 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-07-14]

* **[InfLLM: Training-Free Long-Context Extrapolation for LLMs with an Efficient Context Memory](https://arxiv.org/abs/2402.04617)**
  \[[code](https://github.com/thunlp/InfLLM) ⭐ 406 | 🐛 20 | 🌐 Python | 📅 2024-04-20]

* **[MA-LMM: Memory-Augmented Large Multimodal Model for Long-Term Video Understanding](https://arxiv.org/abs/2404.05726)**
  \[[code](https://github.com/boheumd/MA-LMM) ⭐ 353 | 🐛 18 | 🌐 Python | 📅 2024-07-19]

* **[MemoryLLM: Towards Self-Updatable Large Language Models](https://arxiv.org/abs/2402.04624)**
  \[[code](https://github.com/wangyu-ustc/MemoryLLM) ⭐ 321 | 🐛 5 | 🌐 Python | 📅 2025-07-28]

* [Titans: Learning to Memorize at Test Time](https://arxiv.org/abs/2501.00663)

* [Memory<sup>3</sup>: Language Modeling with Explicit Memory](https://arxiv.org/abs/2407.01178v1)

* [Infinite-LLM: Efficient LLM Service for Long Context with DistAttention and Distributed KVCache](https://arxiv.org/abs/2401.02669)

* [MemServe: Context Caching for Disaggregated LLM Serving with Elastic Memory Pool](https://arxiv.org/abs/2406.17565)

* [WISE: Rethinking the Knowledge Memory for Lifelong Model Editing of Large Language Models](https://arxiv.org/abs/2405.14768/)

* [Ultra-Sparse Memory Network](https://arxiv.org/abs/2411.12364)

#### 🗓️ 2023

* **[Efficient Memory Management for Large Language Model Serving with PagedAttention](https://arxiv.org/abs/2309.06180)**
  \[[code](https://github.com/vllm-project/vllm) ⭐ 89,008 | 🐛 6,537 | 🌐 Python | 📅 2026-08-14]

* **[Augmenting Language Models with Long-Term Memory](https://arxiv.org/abs/2306.07174)**
  \[[code](https://github.com/Victorwz/LongMem) ⭐ 827 | 🐛 12 | 🌐 Python | 📅 2024-03-30]

## 📈 Papers - Memory for Agent Evolution

### 🧭 Reinforcement Learning & Continual Learning

#### 🗓️ 2026

* **[SkillOpt: Executive Strategy for Self-Evolving Agent Skills](https://arxiv.org/abs/2605.23904)**
  \[[code](https://github.com/microsoft/SkillOpt) ⭐ 16,006 | 🐛 29 | 🌐 Python | 📅 2026-08-13]

* **[OpenClaw-RL: Train Any Agent Simply by Talking](https://arxiv.org/abs/2603.10165)**
  \[[code](https://github.com/Gen-Verse/OpenClaw-RL) ⭐ 5,632 | 🐛 74 | 🌐 Python | 📅 2026-05-23]

* **[Memento 2: Learning by Stateful Reflective Memory](https://arxiv.org/abs/2512.22716)**
  \[[code](https://github.com/Agent-on-the-Fly/Memento) ⭐ 2,564 | 🐛 15 | 🌐 Python | 📅 2025-10-05]

* **[Memento-Skills: Let Agents Design Agents](https://arxiv.org/abs/2603.18743)**
  \[[code](https://github.com/Memento-Teams/Memento-Skills) ⭐ 1,541 | 🐛 5 | 🌐 Python | 📅 2026-08-13]

* **[Memory Intelligence Agent](https://arxiv.org/abs/2604.04503)**
  \[[code](https://github.com/ECNU-SII/MIA) ⭐ 792 | 🐛 2 | 🌐 Python | 📅 2026-05-26]

* **[MemSkill: Learning and Evolving Memory Skills for Self-Evolving Agents](https://arxiv.org/abs/2602.02474)**
  \[[code](https://github.com/ViktorAxelsen/MemSkill) ⭐ 560 | 🐛 6 | 🌐 Python | 📅 2026-05-23]

* **[MLEvolve: A Self-Evolving Framework for Automated Machine Learning Algorithm Discovery](https://arxiv.org/abs/2606.06473)**
  \[[code](https://github.com/InternScience/MLEvolve) ⭐ 417 | 🐛 1 | 🌐 Python | 📅 2026-07-14]

* **[SEED: Self-Evolving On-Policy Distillation for Agentic Reinforcement Learning](https://arxiv.org/abs/2607.14777)**
  \[[code](https://github.com/jinyangwu/SEED) ⭐ 230 | 🐛 1 | 🌐 Python | 📅 2026-07-17]
  \[[proj](https://jinyangwu.github.io/seed/)]

* **[PASK: Toward Intent-Aware Proactive Agents with Long-Term Memory](https://arxiv.org/abs/2604.08000)**
  \[[code](https://github.com/xzf-thu/Pask) ⭐ 209 | 🐛 2 | 🌐 Python | 📅 2026-04-17]

* **[MemRL: Self-Evolving Agents via Runtime Reinforcement Learning on Episodic Memory](https://arxiv.org/abs/2601.03192)**
  \[[code](https://github.com/MemTensor/MemRL) ⭐ 166 | 🐛 0 | 🌐 Python | 📅 2026-07-18]

* **[Toward Autonomous Long-Horizon Engineering for ML Research](https://arxiv.org/abs/2604.13018)**
  \[[code](https://github.com/AweAI-Team/AiScientist) ⭐ 144 | 🐛 0 | 🌐 Python | 📅 2026-07-21]

* **[ProcMEM: Learning Reusable Procedural Memory from Experience via Non-Parametric PPO for LLM Agents](https://arxiv.org/abs/2602.01869)**
  \[[code](https://github.com/Miracle1207/ProcMEM) ⭐ 36 | 🐛 5 | 🌐 Python | 📅 2026-05-11]

* **[CASCADE: Case-Based Continual Adaptation for Large Language Models During Deployment](https://arxiv.org/abs/2605.06702)**
  (The DTLBench Paper)
  \[[code](https://github.com/guosyjlu/CASCADE) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2026-05-11]

* **[Learning, Fast and Slow: Towards LLMs That Adapt Continually](https://arxiv.org/abs/2605.12484)**
  \[[code](https://rishabhtiwari.ai/projects/fst/code/)]
  \[[blog](https://gepa-ai.github.io/gepa/blog/2026/05/11/learning-fast-and-slow/)]

* [UniMem: Complementary Episodic-to-Parametric Memory for Boundary-Agnostic Task Streams](https://arxiv.org/abs/2607.26017)

* [Self-Evolving Multi-Agent Systems via Decentralized Memory](https://arxiv.org/abs/2605.22721)

* [Meta-Cognitive Memory Policy Optimization for Long-Horizon LLM Agents](https://arxiv.org/abs/2605.30159)

* [Mem-π: Adaptive Memory through Learning When and What to Generate](https://arxiv.org/abs/2605.21463)

* [Useful Memories Become Faulty When Continuously Updated by LLMs](https://arxiv.org/abs/2605.12978)

* [MEMTIER: Tiered Memory Architecture and Retrieval Bottleneck Analysis for Long-Running Autonomous AI Agents](https://arxiv.org/abs/2605.03675)

* [Neural Garbage Collection: Learning to Forget while Learning to Reason](https://arxiv.org/abs/2604.18002)

* [Why the Brain Consolidates: Predictive Forgetting for Optimal Generalisation](https://arxiv.org/abs/2603.04688)

* [Agentic Memory: Learning Unified Long-Term and Short-Term Memory Management for Large Language Model Agents](https://arxiv.org/abs/2601.01885)

#### 🗓️ 2025

* **[Remember Me, Refine Me: A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution](https://arxiv.org/abs/2512.10696)**
  \[[code](https://github.com/agentscope-ai/ReMe) ⭐ 3,308 | 🐛 30 | 🌐 Python | 📅 2026-08-13]

* **[Memento: Fine-tuning LLM Agents without Fine-tuning LLMs](https://arxiv.org/abs/2508.16153)**
  \[[code](https://github.com/Agent-on-the-Fly/Memento) ⭐ 2,564 | 🐛 15 | 🌐 Python | 📅 2025-10-05]

* **[AgentEvolver: Towards Efficient Self-Evolving Agent System](https://arxiv.org/abs/2511.10395)**
  \[[code](https://github.com/modelscope/AgentEvolver) ⭐ 1,529 | 🐛 21 | 🌐 Python | 📅 2026-04-01]

* **[MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent](https://arxiv.org/abs/2507.02259)**
  \[[code](https://github.com/BytedTsinghua-SIA/MemAgent) ⭐ 1,093 | 🐛 18 | 🌐 Python | 📅 2026-05-12]

* **[General Agentic Memory via Deep Research](https://arxiv.org/abs/2511.18423)**
  \[[code](https://github.com/VectorSpaceLab/general-agentic-memory/) ⭐ 859 | 🐛 3 | 🌐 Python | 📅 2026-03-14]

* **[End-to-End Test-Time Training for Long Context](https://arxiv.org/abs/2512.23675)**
  \[[code](https://github.com/test-time-training/e2e) ⭐ 660 | 🐛 1 | 🌐 Python | 📅 2026-02-15]

* **[ML-Master: Towards AI-for-AI via Integration of Exploration and Reasoning](https://arxiv.org/abs/2506.16499)**
  \[[code](https://github.com/sjtu-sai-agents/ML-Master) ⭐ 441 | 🐛 7 | 🌐 Python | 📅 2026-03-29]

* **[MemEvolve: Meta-Evolution of Agent Memory Systems](https://arxiv.org/abs/2512.18746)**
  \[[code](https://github.com/bingreeky/MemEvolve) ⭐ 259 | 🐛 3 | 🌐 Python | 📅 2026-05-05]

* **[Mem-α: Learning Memory Construction via Reinforcement Learning](https://arxiv.org/abs/2509.25911)**
  \[[code](https://github.com/wangyu-ustc/Mem-alpha) ⭐ 222 | 🐛 13 | 🌐 Python | 📅 2025-12-25]

* **[EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle](https://arxiv.org/abs/2510.16079)**
  \[[code](https://github.com/KnowledgeXLab/EvolveR) ⭐ 106 | 🐛 0 | 🌐 Python | 📅 2026-05-08]

* **[Learning on the Job: An Experience-Driven, Self-Evolving Agent for Long-Horizon Tasks](https://arxiv.org/abs/2510.08002)**
  \[[code](https://github.com/KnowledgeXLab/MUSE) ⭐ 99 | 🐛 2 | 🌐 Python | 📅 2026-07-20]

* **[FLEX: Continuous Agent Evolution via Forward Learning from Experience](https://arxiv.org/abs/2511.06449)**
  \[[code](https://github.com/GenSI-THUAIR/FLEX) ⭐ 85 | 🐛 2 | 🌐 Python | 📅 2026-06-09]

* **[Goal-Directed Search Outperforms Goal-Agnostic Memory Compression in Long-Context Memory Tasks](https://arxiv.org/abs/2511.21726)**
  \[[code](https://arxiv.org/abs/2511.21726)]

* [Beyond Heuristics: A Decision-Theoretic Framework for Agent Memory Management](https://arxiv.org/abs/2512.21567)

* [Nested Learning: The Illusion of Deep Learning Architecture](https://abehrouz.github.io/files/NL.pdf)
  \[[blog](https://research.google/blog/introducing-nested-learning-a-new-ml-paradigm-for-continual-learning/)]

* [LightSearcher: Efficient DeepSearch via Experiential Memory](https://www.arxiv.org/abs/2512.06653)

* [Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning](https://arxiv.org/abs/2508.19828)

* [Latent Learning: Episodic Memory Complements Parametric Learning by Enabling Flexible Reuse of Experiences](https://arxiv.org/abs/2509.16189)

* [Evo-Memory: Benchmarking LLM Agent Test-time Learning with Self-Evolving Memory](https://arxiv.org/abs/2511.20857)

* [ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory](https://arxiv.org/abs/2509.25140)

* [Long Term Memory: The Foundation of AI Self-Evolution](https://arxiv.org/abs/2410.15665)

* [REFRAG: Rethinking RAG based Decoding](https://arxiv.org/abs/2509.01092)

* [MemGen: Weaving Generative Latent Memory for Self-Evolving Agents](https://arxiv.org/abs/2509.24704)

* [ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization](https://arxiv.org/abs/2509.13313)

* [MARC: Memory-Augmented RL Token Compression for Efficient Video Understanding](https://arxiv.org/pdf/2510.07915)

* [Continual Learning via Sparse Memory Finetuning](https://arxiv.org/abs/2510.15103)

* [Task-Core Memory Management and Consolidation for Long-term Continual Learning](https://arxiv.org/abs/2505.09952)

### 🧩 Context Engineering & Harness Engineering

#### 🗓️ 2026

* **[LCM: Lossless Context Management](https://papers.voltropy.com/LCM)**
  \[[code](https://github.com/Martian-Engineering/lossless-claw) ⭐ 4,884 | 🐛 219 | 🌐 TypeScript | 📅 2026-08-11]

* **[Code as Agent Harness](https://arxiv.org/abs/2605.18747)**
  \[[code](https://github.com/YennNing/Awesome-Code-as-Agent-Harness-Papers) ⭐ 641 | 🐛 12 | 📅 2026-05-20]

* **[CL-bench: A Benchmark for Context Learning](https://arxiv.org/abs/2602.03587)**
  \[[code](https://github.com/Tencent-Hunyuan/CL-bench) ⭐ 576 | 🐛 15 | 🌐 Python | 📅 2026-05-12]

* **[SWE-Pruner: Self-Adaptive Context Pruning for Coding Agents](https://arxiv.org/abs/2601.16746)**
  \[[code](https://github.com/Ayanami1314/swe-pruner) ⭐ 308 | 🐛 2 | 🌐 Python | 📅 2026-06-30]

* **[Self-Harness: Harnesses That Improve Themselves](https://arxiv.org/abs/2606.09498)**
  \[[code](https://github.com/qzzqzzb/Self-Harness) ⭐ 67 | 🐛 1 | 🌐 Python | 📅 2026-07-02]

* [Is Grep All You Need? How Agent Harnesses Reshape Agentic Search](https://arxiv.org/abs/2605.15184)

* [M\*: Every Task Deserves Its Own Memory Harness](https://arxiv.org/abs/2604.11811)

#### 🗓️ 2025

* **[AgentFold: Long-Horizon Web Agents with Proactive Context Management](https://arxiv.org/abs/2510.24699)**
  \[[code](https://github.com/Alibaba-NLP/DeepResearch) ⭐ 19,828 | 🐛 92 | 🌐 Python | 📅 2026-02-27]

* **[Everything is Context: Agentic File System Abstraction for Context Engineering](https://arxiv.org/abs/2512.05470)**
  \[[code](https://github.com/AIGNE-io/aigne-framework) ⭐ 369 | 🐛 17 | 🌐 TypeScript | 📅 2026-01-25]

* **[ACON: Optimizing Context Compression for Long-horizon LLM Agents](https://arxiv.org/abs/2510.00615)**
  \[[code](https://github.com/microsoft/acon) ⭐ 100 | 🐛 6 | 🌐 Python | 📅 2025-10-14]

* [Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models](https://arxiv.org/abs/2510.04618)

## 🔬 Papers - Memory in Cognitive Science

#### 🗓️ 2026

* **[A Neural Network Model of Free Recall Learns Multiple Memory Strategies](https://www.nature.com/articles/s42256-026-01274-0)**
  \[[code](https://github.com/Veritaria/rnn-free-recall) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2026-07-13]

* [Subspace Communication in the Hippocampal–Retrosplenial Axis](https://www.nature.com/articles/s41586-026-10481-z)

* [A Neural State Space for Episodic Memories](https://www.cell.com/trends/cognitive-sciences/fulltext/S1364-6613\(25\)00284-0)

* [Dopaminergic Processes Predict Temporal Distortions in Event Memory](https://www.nature.com/articles/s41467-026-69950-8)

* [Awareness as the Heart of Working Memory](https://www.sciencedirect.com/science/article/pii/S1364661326000756)

* [Neural Activations and Representations during Episodic versus Semantic Memory Retrieval](https://www.nature.com/articles/s41562-025-02390-4)

* [Distinct Neuronal Populations in the Human Brain Combine Content and Context](https://www.nature.com/articles/s41586-025-09910-2)

#### 🗓️ 2025

* [Neural Population Activity for Memory: Properties, Computations, and Codes](https://www.cell.com/neuron/fulltext/S0896-6273\(25\)00854-2)

* [How Prediction Error Drives Memory Updating: Role of Locus Coeruleus–Hippocampal Interactions](https://www.cell.com/trends/neurosciences/abstract/S0166-2236\(25\)00189-4)

* [Towards Large Language Models with Human-Like Episodic Memory](https://www.cell.com/trends/cognitive-sciences/abstract/S1364-6613\(25\)00179-2)

#### 🗓️ 2024

* [A Generative Model of Memory Construction and Consolidation](https://www.nature.com/articles/s41562-023-01799-z)

***

## 🔒 Memory Security & Defense

* **[Agent Memory Guard](https://owasp.org/www-project-agent-memory-guard/)**
  \[[code](https://github.com/OWASP/www-project-agent-memory-guard) ⭐ 124 | 🐛 24 | 🌐 Python | 📅 2026-08-14]
  \[[pypi](https://pypi.org/project/agent-memory-guard/)]
  *OWASP runtime defense layer that screens agent memory writes for poisoning before they reach the agent — multi-layer validation with semantic anomaly detection, entropy scoring, provenance verification, and cross-reference and temporal checks.*

* **[inspeximus (formerly mnemo) poisoning probes](https://github.com/DanceNitra/agora/tree/main/research/probes) ⭐ 3 | 🐛 5 | 🌐 Python | 📅 2026-08-13**
  \[[attack](https://github.com/DanceNitra/agora/blob/main/research/probes/memory_defense_layer_probe.py) ⭐ 3 | 🐛 5 | 🌐 Python | 📅 2026-08-13]
  \[[defense](https://github.com/DanceNitra/agora/blob/main/research/probes/memory_gate_defense_probe.py) ⭐ 3 | 🐛 5 | 🌐 Python | 📅 2026-08-13]
  *Runnable probe scripts demonstrating that provenance written into a memory record is forgeable, and that a retrieval-time corroboration gate raises the cost of memory-poisoning attacks.*

* [From Untrusted Input to Trusted Memory: A Systematic Study of Memory Poisoning Attacks in LLM Agents](https://arxiv.org/abs/2606.04329)
  (The MPBench Paper)

***

## 📰 Articles

#### 🗓️ 2026

* [Harness Engineering for Self-Improvement](https://lilianweng.github.io/posts/2026-07-04-harness/)

* [Why Character.AI Forgets You — And What Persistent Memory Actually Requires](https://web.archive.org/web/20260429101535/https://blog.kinthai.ai/why-character-ai-forgets-you-persistent-memory-architecture) (archived; original site currently unreachable)

* [221 Agents: Multi-Agent Coordination Lessons](https://web.archive.org/web/20260427040129/https://blog.kinthai.ai/221-agents-multi-agent-coordination-lessons) (archived; original site currently unreachable)

* [OpenClaw Multi-Tenancy: Why VM-Per-User Does Not Scale](https://web.archive.org/web/20260429092735/https://blog.kinthai.ai/openclaw-multi-tenancy-why-vm-per-user-doesnt-scale) (archived; original site currently unreachable)

#### 🗓️ 2025

* [Survey of AI Agent Memory Frameworks](https://www.graphlit.com/blog/survey-of-ai-agent-memory-frameworks)

#### 🗓️ 2024

* [Memory in Language Model-Enabled Agents](https://yuweisunn.github.io/blog-1-06-24.html)

* [Mastering LLM Memory: A Comprehensive Guide](https://www.strongly.ai/blog/mastering-llm-memory-a-comprehensive-guide.html)

#### 🗓️ 2023

* [LLM Powered Autonomous Agents](https://lilianweng.github.io/posts/2023-06-23-agent/)

***

## 👥 Workshops

#### 🗓️ 2026

* [ICLR 2026](https://iclr.cc/Conferences/2026): [Workshop on Memory for LLM-Based Agentic Systems (MemAgents)](https://sites.google.com/view/memagent-iclr26/)
  \[[schedule](https://sites.google.com/view/memagent-iclr26/schedule)]

#### 🗓️ 2025

* [ACL 2025](https://2025.aclweb.org/): [The First Workshop on Large Language Model Memorization (L2M2)](https://sites.google.com/view/memorization-workshop)
  \[[proceedings](https://aclanthology.org/volumes/2025.l2m2-1/)]

***

## 📑 Citation

To cite this collection itself, use the metadata in [`CITATION.cff`](CITATION.cff) (GitHub's "Cite this repository" button), or:

```bibtex
@misc{zhang2025awesomeagentmemory,
        author = {Zhang, Dell and Sun, Changzhi and Luo, Jixiang and Chen, Xiangyu and Li, Xuelong},
        title = {Awesome Agent Memory: Curated Systems, Benchmarks, and Papers on Memory for {LLMs}/{MLLMs}},
        year = {2025},
        howpublished = {\url{https://github.com/TeleAI-UAGI/Awesome-Agent-Memory}}
}
```

This list grew out of the maintainers' SIGIR-AP 2025 tutorial, which you can cite as the related publication:

```bibtex
@inproceedings{zhangConversationalAgentsRAG2025,
        author = {Zhang, Dell and Feng, Yue and Liu, Haiming and Sun, Changzhi and Luo, Jixiang and Chen, Xiangyu and Li, Xuelong},
        title = {Conversational Agents: From {RAG} to {LTM}},
        year = {2025},
        isbn = {9798400722189},
        doi = {10.1145/3767695.3769671},
        booktitle = {Proceedings of the 2025 Annual International ACM SIGIR Conference on Research and Development in Information Retrieval in the Asia Pacific Region (SIGIR-AP)},
        pages = {447–452},
        location = {China}
}
```

***

## Star History

<a href="https://github.com/TeleAI-UAGI/Awesome-Agent-Memory/stargazers"><picture> <source media="(prefers-color-scheme: dark)" srcset="assets/star-history-dark.svg"> <img alt="Star history chart of TeleAI-UAGI/Awesome-Agent-Memory" src="assets/star-history-light.svg"> </picture></a>

<sub>Regenerated weekly by [a scheduled workflow](.github/workflows/star-history.yml); the previous [star-history.com](https://www.star-history.com/) live chart broke when GitHub restricted the stargazers API to repo admins and collaborators in June 2026.</sub>

***

<div align="center">

**If you find this page helpful, please give it a ⭐️ — starring also keeps updates in your GitHub feed.**

Made with ❤️ by [Bloo-Mind AI Ltd](https://www.bloo-mind.ai/) and the Ubiquitous AGI team at TeleAI.

</div>

<div align="center" style="margin-top: 10px;">
    <a href="https://www.bloo-mind.ai/"><img src="assets/bloo-mind.png" alt="Bloo-Mind Logo" width="120px" /></a>
    &nbsp;&nbsp;&nbsp;
    <img src="assets/TeleAI.png" alt="TeleAI Logo" width="120px" />
</div>

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-14._
