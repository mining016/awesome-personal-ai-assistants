# Awesome Personal AI Assistants [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Stars](https://img.shields.io/github/stars/mining016/awesome-personal-ai-assistants?style=social)](https://github.com/mining016/awesome-personal-ai-assistants)

A curated list of awesome personal AI assistants, local-first autonomous agents, self-hosted AI tools, and action-oriented bots (featuring OpenClaw 🦞 and similar projects).

> Inspired by the awesome lists movement. Focused on privacy-first, local-running, task-executing AI agents that go beyond chat-handling emails, calendars, shell commands, web browsing, file ops, and proactive workflows. Unlike broader AI agent lists, this emphasizes personal use cases (e.g., JARVIS-style assistants on your own hardware, via messaging apps like WhatsApp or iMessage). OpenClaw (formerly Moltbot/Clawdbot) is highlighted as the flagship due to its viral growth and extensibility in early 2026.

## Contents

- [OpenClaw Ecosystem](#openclaw-ecosystem)
- [Other Local/Self-Hosted Personal AI Assistants](#other-localself-hosted-personal-ai-assistants)
- [Frameworks and Toolkits for Building Personal Agents](#frameworks-and-toolkits-for-building-personal-agents)
- [Skills, Plugins, and Extensions](#skills-plugins-and-extensions)
- [Security and Best Practices](#security-and-best-practices)
- [Related Awesome Lists](#related-awesome-lists)

## OpenClaw Ecosystem

The flagship: OpenClaw 🦞 is an open-source, self-hosted personal AI assistant that runs locally and performs real actions via messaging apps (WhatsApp, Telegram, etc.). It exploded in popularity in early 2026 for its extensibility and privacy focus.

**Name history (all the same project!)**:  
- Originally released in late 2025 as **Clawdbot** (inspired by Anthropic's Claude "Clawd" mascot).  
- Renamed to **Moltbot** shortly after viral growth due to a trademark concern from Anthropic (to avoid confusion with their Claude branding). "Molting" symbolized growth, like a lobster shedding its shell.  
- Final rebrand in late January 2026 to **OpenClaw** — emphasizing open-source roots while keeping the lobster theme ("Claw" + "Open").  

This triple rebrand happened quickly amid hype, security discussions, and even some scams exploiting old names. All versions refer to the identical core software—just evolving branding.

### Core Resources
- **[OpenClaw](https://github.com/openclaw/openclaw)** — Core repo: Local AI agent for task execution, long-term memory, and integrations. Stars: ~100k (as of early 2026). Official site: [openclaw.ai](https://openclaw.ai).  
- **[OpenClaw Discord](https://discord.gg/openclaw-community)** — Active community for setups, troubleshooting, and sharing skills.  
- **[OpenClaw Security Guide](https://openclaw.ai/docs/security)** — Official best practices for sandboxing and key management.  

### Community Platforms & Registries
- **[ClawHub](https://www.clawhub.com/)** — The skill dock/registry for OpenClaw agents: Upload, version, and search AgentSkills bundles (like npm for AI tools). Features highlighted skills (e.g., Trello, Slack, Calendar) and easy install commands (e.g., `npx clawhub@latest install`). Stars: N/A (platform, not repo).  
- **[MoltBook](https://www.moltbook.com/)** — Social network exclusively for AI agents (humans observe only): Agents share, discuss, upvote content, and interact autonomously. Viral "front page of the agent internet" built around OpenClaw/Moltbot skills. Beta in early 2026 with millions of agent posts.  

### Popular Forks & Setups
- **[awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills)** — Curated 700+ skills (e.g., email, browser, finance). Stars: ~5k. Focus: Community extensions.  
- **[openclaw-voice](https://github.com/community/openclaw-voice)** — Voice integration via Whisper/STT.  
- **[openclaw-multi-agent](https://github.com/dev/openclaw-multi-agent)** — Examples for team-of-agents workflows.  

## Other Local/Self-Hosted Personal AI Assistants

Curated projects similar to OpenClaw: Privacy-focused, offline-capable, action-oriented for personal productivity. Expanded entries include community resources where available.

- **[Open Interpreter](https://github.com/KillianLucas/open-interpreter)** — Local code execution agent; runs shell commands safely on your machine. Stars: ~30k. Why awesome: Turns natural language into real computer actions with strong local model support.
  - **Popular YouTube Videos / Tutorials**:
    - [Open Interpreter: Beginners Tutorial with 10+ Use Cases YOU CAN'T MISS](https://www.youtube.com/watch?v=W-VwN0n4d9Y) — Step-by-step setup, local LLM integration, real tasks (dark mode toggle, app creation).
    - [Open Interpreter in 7 Minutes](https://www.youtube.com/watch?v=nL2G6Kz4BN0) — Quick overview of local code interpreter basics.
    - [Open Interpreter Tutorial (UPDATED March 2024)](https://www.youtube.com/watch?v=sb40Tqj90Q0) — Anaconda install, fast mode, local models.
    - [AI Controls the COMPUTER - Open-Interpreter FULL TUTORIAL](https://www.youtube.com/watch?v=01tQLn_RRcE) — Installation, troubleshooting, local models, use cases.
    - [Open Interpreter Secrets Revealed: Setup Guide & Examples](https://www.youtube.com/watch?v=E0ujWJOQOeQ) — Optimal setup, examples (file navigation, system prefs).
  - **Courses / Structured Learning**:
    - Official docs: Comprehensive README + examples for safe/local usage.
  - **Reddit Discussions / Communities**:
    - r/LocalLLaMA: Threads like ["Has anyone tried open interpreter?"](https://www.reddit.com/r/LocalLLaMA/comments/1cpw1ye/has_anyone_tried_open_interpreter) — Real user experiences, Linux dependency fixes.
    - Active mentions in r/LocalLLM and agent-focused subs.

- **[Leon](https://github.com/leon-ai/leon)** — Open-source personal assistant; fully offline, privacy-first with speech-to-text and modular skills. Stars: ~17k. Why awesome: Server-based, extensible for custom personal tasks.
  - **Popular YouTube Videos / Tutorials**:
    - [[Preview] 5 Years Later... Let's Build Me Together. Leon](https://www.youtube.com/watch?v=6CInSt6pTVA) — Overview of rewritten core, new engines, community building.
  - **Courses / Structured Learning**:
    - Official Docs: [Introduction & Installation](https://docs.getleon.ai/) — Step-by-step CLI install, prerequisites, running Leon locally.
    - [Leon CLI & Setup Guide](https://docs.getleon.ai/) — Modular architecture, skill creation.
  - **Reddit Discussions / Communities**:
    - r/node: Older but relevant thread on Leon as open-source assistant.
    - Discord community (linked in repo/docs) for active support.

- **[PrivateGPT](https://github.com/imartinez/privateGPT)** — Interact with documents offline, 100% private RAG-style querying. Stars: ~40k. Why awesome: No data leaves your machine; great for personal knowledge bases.
  - **Popular YouTube Videos / Tutorials**:
    - [How TO SetUp and USE PrivateGPT | FULLY LOCAL | 100% PRIVATE](https://www.youtube.com/watch?v=VEQ8mxv2MHY) — Complete local install and usage demo.
    - [How To Install PrivateGPT - Chat With PDF, TXT, and CSV Files Privately!](https://www.youtube.com/watch?v=jxSPx1bfl2M) — Quick setup guide for document chatting.
  - **Courses / Structured Learning**:
    - Official repo README + install guides (detailed vs quick versions).
    - Medium/Mac guide: [Setup your own PrivateGPT on Mac](https://medium.com/@effendy_59676/setup-your-own-privategpt-on-mac-c17d75bbdde3) — Poetry/Ollama integration.
  - **Reddit Discussions / Communities**:
    - r/LocalLLaMA: Multiple threads e.g., ["Just sharing some quick tips to painlessly install PrivateGPT on Windows with WSL"](https://www.reddit.com/r/LocalLLaMA/comments/1923f4k/just_sharing_some_quick_tips_to_painlessly), performance tweaks, UI + NVIDIA help.

- **[LocalGPT](https://github.com/PromtEngineer/localGPT)** — Chat with documents locally using GPT models; no data leaks. Stars: ~50k.
  - (No major dedicated video/course resources beyond overlapping PrivateGPT guides; community discussions often merge with PrivateGPT in r/LocalLLaMA.)

- **[DB-GPT](https://github.com/csunny/DB-GPT)** — Local GPT for secure data/environment interaction. Stars: ~20k.
  - (Primarily repo-focused; limited standalone tutorials/videos.)

- **[AgentRunner.ai](https://github.com/agentrunner/agentrunner)** — Train autonomous agents locally with GPT-4. Stars: ~10k.
- **[HyperWrite](https://github.com/hyperwrite/hyperwrite)** — Personal writing/editing assistant; local options. Stars: ~15k.
- **[AI Agents](https://github.com/ai-agents/ai-agents)** — Productivity-focused local agents. Stars: ~8k.


## Frameworks and Toolkits for Building Personal Agents

Tools to create your own local assistants.

- [CrewAI](https://github.com/joaomdmoura/crewAI) - Framework for multi-agent orchestration; local-friendly. Stars: ~25k.
- [LangGraph](https://github.com/langchain-ai/langgraph) - Build stateful agents with local LLMs. Stars: ~15k.
- [Ollama](https://github.com/jmorganca/ollama) - Run local LLMs for agent backends. Stars: ~50k.
- [LM Studio](https://github.com/lmstudio-ai/lm-studio) - Discover/run local models; agent integration. Stars: ~20k.
- [LocalAI](https://github.com/go-skynet/LocalAI) - OpenAI-compatible API for local inference. Stars: ~18k.
- [SuperAGI](https://github.com/TransformerOptimus/SuperAGI) - Build/deploy local agents. Stars: ~10k.
- [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) - Autonomous agent; local forks available. Stars: ~177k (broad appeal).
- [BabyAGI](https://github.com/yoheinakajima/babyagi) - Task-driven agent framework; local use. Stars: ~15k.

## Skills, Plugins, and Extensions

Extensible add-ons for personal agents (general + OpenClaw-specific).

- General Skills/Toolkits:
  - [Browser Tools](https://github.com/agent-tools/browser) - Web scraping/automation for agents.
  - [Email/Calendar Wrappers](https://github.com/productivity/email-agent) - API integrations for Gmail, Outlook.
  - [Shell Command Toolkit](https://github.com/open-interpreter/shell) - Safe local execution.
  - [File I/O Plugins](https://github.com/agent-file/file-ops) - Read/write local files.
  - [Crypto/On-Chain Skills](https://github.com/blockchain/agent-crypto) - Wallet management, transactions.
- OpenClaw-Specific (from awesome-openclaw-skills):
  - Productivity (42 items): Task management, reminders.
  - AI & LLMs (38 items): Model switching, fine-tuning.
  - Notes & PKM (44 items): Obsidian/Evernote integrations.
  - Browser & Automation (11 items): Puppeteer-based.
  - Security (6 items): Password managers.

## Security and Best Practices

Critical for local agents with access to personal data.

- Run in a sandbox/VM (e.g., Docker, VirtualBox).
- Use dedicated API keys/emails; never production accounts.
- Isolate hardware (e.g., Mac Mini for OpenClaw).
- Mitigate prompt injection: Validate inputs.
- Review skills/plugins before install.
- Resources: [OpenClaw Security Docs](https://openclaw.ai/security), [OWASP AI Guide](https://owasp.org/www-project-top-10-for-large-language-model-applications/).

## Related Awesome Lists

Broader/more specialized lists for cross-reference:

- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents) - General autonomous agents; includes personal (web version with filters).
- [awesome-agents](https://github.com/kyrolabs/awesome-agents) - Agent-building tools; some local emphasis.
- [awesome-local-ai](https://github.com/janhq/awesome-local-ai) - Local AI tools; agents subsection.
- [awesome-ai-agents (slavakurilyak)](https://github.com/slavakurilyak/awesome-ai-agents) - 300+ agentic resources; top projects by stars.

## Contributing

Contributions welcome! Add open-source, local-first projects via PR. Criteria:
- Must emphasize personal use, privacy, local execution.
- Actively maintained (updates in last 6 months).
- Real task capabilities (not just chatbots).
- Format: - `**[Name](link)**` - Short desc. Stars: ~Xk.
See [CONTRIBUTING.md](CONTRIBUTING.md) for details.


