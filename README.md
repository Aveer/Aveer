# Aveer

**AI Systems · Agentic Software Engineering · Local LLMs · Embedded Systems**

I build practical AI infrastructure, developer tooling and embedded systems - with a strong focus on **local-first AI, agentic coding workflows and physical device integration**.

My main work currently sits at the intersection of:

`LLM infrastructure` · `AI agents` · `developer tooling` · `ESP32 / IoT` · `robotics`

---

## LM-Nexus

**Local-first AI workspace and control center for developers.**

LM-Nexus is my main project. It combines local model management, chat, agents, terminals, files, knowledge, monitoring and system tooling in one browser-based environment.

Highlights:

- managed local `llama.cpp` / `llama-server` inference
- GGUF model discovery and management
- OpenAI-compatible local APIs
- persistent multi-provider chat
- custom Agent Runtime with tools, skills and delegation
- approval-gated agent actions
- browser PTY / Windows ConPTY terminals
- file editing and knowledge management
- CPU / RAM / GPU / VRAM monitoring
- Docker and shell-based integrations
- modular extension and package system
- command-line access to models, chat and modules

**Python · FastAPI · Vue 3 · TypeScript · Vite · Docker · llama.cpp**

> Currently private and under active development.

---

## Agentic software engineering

I spend a large part of my development time experimenting with **multi-agent software engineering** - orchestration, delegation, reusable skills, configuration layering, verification and long-running coding workflows.

### oh-my-opencode-slim

I'm an active upstream contributor to [oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim), an OpenCode multi-agent orchestration framework. My contributions focus on agent execution and configuration for real-world local AI workflows.

I keep a public [fork](https://github.com/Aveer/oh-my-opencode-slim) as my upstream contribution workspace - a place for feature branches and PR history while contributing changes back to the main project, rather than as a separate long-term distribution.

So far I've authored three substantial upstream PRs, with two merged:

- **[PR #1179 - same-provider task scheduling](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1179)** - merged. Adds an opt-in provider policy that converts same-provider background delegation to foreground execution, avoiding expensive model/KV-context switching on constrained local inference backends.
- **[PR #1190 - composable per-agent skill configuration](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1190)** - merged. Adds `skills_add` / `skills_remove` across layered global, project and preset configuration, including runtime resolution, wildcard/exclusion semantics, schema support, regression coverage and integration tests.
- **[PR #1204 - automatic project-local skill discovery](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1204)** - open. Adds `skills_include_local` for automatically granting Agent Skills discovered under a project's `.opencode/skills`, with config layering, exclusion precedence, canonical-path boundary checks and integration coverage.

### Agent Skills

[`Aveer/skills`](https://github.com/Aveer/skills) is my source-of-truth repository for reusable Agent Skills shared across OpenCode and other compatible coding environments.

It includes workflows for:

- multi-agent deep work
- architecture and codebase exploration
- systematic debugging
- verification planning
- repository governance
- worktrees
- TypeScript / Vue development
- product and UX reasoning

---

## Nexus Devices

I'm extending the Nexus ecosystem into physical hardware through a shared ESP32 firmware platform.

Current capabilities include:

- distributed device discovery
- capability-based device APIs
- authenticated device-to-device communication
- HMAC-SHA256 fabric authentication
- capability routing
- signed OTA updates
- runtime hardware configuration
- Zigbee coordination
- mmWave presence radar
- servo control
- OLED, distance and temperature sensors
- embedded dashboards and JSON APIs

The long-term direction is to give AI agents a controlled interface to **real-world devices and robotics hardware**.

**C · ESP-IDF · ESP32 · ESP32-C5 · Wi-Fi · Zigbee · mDNS**

---

## Selected public projects

### [OpenZeus](https://github.com/Aveer/OpenZeus)

OpenCode setup, validation and asset-generation toolkit.

It can bootstrap project configuration, generate agents/skills/commands, detect config drift, validate CI state and perform safe upgrades with backups.

```bash
npm install -g openzeus
```

---

### [Korean Vocabulary Extractor](https://github.com/Aveer/korean-vocabulary-extractor)

Local Korean vocabulary extraction and study application.

Features include morphological analysis, TOPIK-aware filtering, an offline Korean-English dictionary, SQLite study data, lightweight spaced review and Anki-compatible export.

**Python · FastAPI · Vue · SQLite**

---

### [The Settlers 7 CPU Optimizer](https://github.com/Aveer/The-Settlers-7-CPU-Optimizer)

A dependency-free **PowerShell** utility that improves *The Settlers 7* performance by adjusting process priority and CPU affinity to avoid logical sibling threads.

The current maintained implementation is PowerShell-first; the old Python-packaged executable is retained only as a legacy option.

---

## Tech

**AI / Agents**  
`Local LLMs` · `llama.cpp` · `Agent orchestration` · `Tool calling` · `Agent Skills` · `OpenCode`

**Backend**  
`Python` · `FastAPI` · `Pydantic` · `pytest` · `SQLite`

**Frontend**  
`Vue 3` · `TypeScript` · `JavaScript` · `Vite` · `Pinia`

**Systems**  
`Docker` · `PowerShell` · `Linux / WSL` · `Windows` · `GitHub Actions`

**Embedded**  
`C` · `ESP-IDF` · `ESP32` · `Wi-Fi` · `Zigbee` · `Sensors` · `Robotics`

---

## Current interests

Local AI infrastructure · agentic coding · multi-agent systems · developer tooling · embedded systems · robotics · physical-world AI interfaces
