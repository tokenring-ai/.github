# TokenRing AI

**AI-powered tools for coding and content creation**

TokenRing AI builds practical, agent-driven software for people who want to create faster with AI. Our ecosystem centers around:

- **TokenRing One** — The all-in-one AI assistant for development and content creation
- **llama-scale** — An OpenAI-compatible LLM router for locally hosted inference servers

TokenRing One sits on top of a modular TypeScript monorepo with a large shared package ecosystem for agents, workflows, research, storage, publishing, automation, and real-time interfaces. llama-scale is a lightweight Rust service that unifies local model backends behind a single endpoint.

## Products

### [TokenRing One](https://github.com/tokenring-ai/one)
A unified AI-powered platform built for developers and creators who want to work directly with their codebase and content through chat, commands, automation, and specialized agents.

**What it does:**
- **Coding:** Helps with editing, refactoring, testing, and debugging
- **Writing:** Assists with article writing, editing, and publishing workflows
- **Research:** Supports web search, Wikipedia, and information retrieval
- **Infrastructure:** Works locally with your code, databases, and publishing platforms
- **Integration:** Connects with git, Docker, Kubernetes, WordPress, Ghost, and more

**Highlights:**
- Multiple AI providers (OpenAI, Anthropic, Google, Groq, Cerebras, DeepSeek, and more)
- Interactive CLI and web interface
- Specialized agents for frontend, backend, testing, DevOps, architecture, security, and content
- WebSocket and remote communication support
- Strong local-first development and workflow state
- Agent-based content creation and code orchestration

### [llama-scale](https://github.com/tokenring-ai/llama-scale)
A simple, Rust-based **OpenAI-compatible LLM router** for locally hosted inference servers. Point your apps at one endpoint and llama-scale forwards each request to Ollama, llama.cpp, vLLM, LM Studio, or any combination of them.

**What it does:**
- **Routing:** Load-balances across backend replicas with least-connections selection
- **Session affinity:** Keeps multi-turn conversations pinned to the same backend so context stays warm
- **Failover:** Health-checks backends and fails over by fallback tier when hosts are down or saturated
- **Compatibility:** Exposes a standard OpenAI `/v1` API so existing clients work without changes
- **Ops:** Supports Docker, Kubernetes, systemd packages, TLS, multi-user API keys, and Prometheus metrics

**Highlights:**
- OpenAI-compatible passthrough for any `/v1/*` path (streaming supported)
- Conversation-sticky routing with no client changes
- Merged `/models` endpoint with background refresh and per-backend aliases
- Per-backend concurrency caps and stream-aware timeouts
- Bearer API key auth (including multi-user model allowlists and rate limits)
- Install via script, npm/npx, prebuilt binaries, Cargo, Docker, or `.deb`/`.rpm`

## Shared Platform

TokenRing One is powered by the broader TokenRing AI monorepo: a modular TypeScript ecosystem with 50+ packages for agent orchestration, AI clients, storage, filesystem abstraction, research, scripting, workflow execution, publishing, cloud services, and frontend interfaces.

## Core Capabilities

Across the TokenRing platform, the ecosystem includes:

- **Agent orchestration** for specialized AI workflows
- **Multi-provider AI support** across leading commercial and open models
- **Local LLM routing** with OpenAI-compatible load balancing and session affinity
- **Local and cloud filesystem support**
- **Research and web search tooling**
- **Database and persistence layers**
- **Publishing and communication integrations**
- **CLI, web UI, and API-driven interfaces**
- **Workflow automation and scripting**

## Technology

- **Languages:** TypeScript, JavaScript, Node.js, Bun, Rust
- **Frontend:** React, Vite
- **Infrastructure:** Docker, Kubernetes, WebSockets, Fastify, systemd
- **Storage:** SQLite, MySQL, PostgreSQL, S3
- **AI:** OpenAI, Anthropic, Google, Groq, Cerebras, DeepSeek, Ollama, llama.cpp, vLLM, LM Studio, and more

## Getting Started

- Explore **[TokenRing One](https://github.com/tokenring-ai/one)** for the complete package ecosystem
- Explore **[llama-scale](https://github.com/tokenring-ai/llama-scale)** to route local LLM traffic through one OpenAI-compatible endpoint

## Documentation

- [TokenRing One README](https://github.com/tokenring-ai/one#readme)
- [llama-scale README](https://github.com/tokenring-ai/llama-scale#readme)

## Contributing

We welcome contributions across our open-source projects. Check the individual repositories for setup instructions, contribution guidelines, and package-specific documentation.

## Links

- **Website:** [tokenring.ai](https://tokenring.ai)
- **GitHub:** [github.com/tokenring-ai](https://github.com/tokenring-ai)

---

**TokenRing AI** builds practical agent-driven tools for developers and content creators.
