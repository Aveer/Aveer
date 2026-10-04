# Aver

**AI Systems · Agentic Software Engineering · Local LLMs · Embedded Systems**

I build local AI infrastructure, developer tools and embedded systems. Most of my current work is around **local LLMs, agentic coding workflows and connecting software agents to physical devices**.

`LLM infrastructure` · `AI agents` · `developer tooling` · `ESP32 / IoT` · `robotics`

---

## LM-Nexus

**Local-first AI workspace and control center.**

LM-Nexus is my main project. It brings local model management, chat, agents, terminals, files, knowledge, monitoring and system tooling into one browser-based environment.

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

I spend a lot of my development time on **agentic software engineering**: orchestration, delegation, reusable skills, configuration layering, execution semantics, verification and long-running coding workflows.

### oh-my-opencode-slim

I'm an active upstream contributor to [oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim), an OpenCode multi-agent orchestration framework. My work there covers agent runtime behavior, configuration and Agent Skills, the native Companion UI, testing and CI.

I use my public [fork](https://github.com/Aveer/oh-my-opencode-slim) as a contribution workspace for branches and PRs going back upstream, not as a separate distribution.

Selected upstream work:

- **Local inference scheduling - [#1179](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1179):** same-provider background tasks can opt into foreground execution to avoid unnecessary model/KV-context switching on constrained local inference backends.
- **Agent Skills configuration - [#1190](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1190), [#1204](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1204):** composable per-agent skill additions/removals and automatic project-local skill discovery, with layered config semantics and path-boundary checks.
- **Native Companion controls - [#1419](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1419), [#1421](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1421):** scoped Project / Global / Inherit preset switching plus live agent/model and waiting-input state.
- **Companion CI - [#1424](https://github.com/alvinunreal/oh-my-opencode-slim/pull/1424):** pull-request validation for the Rust Companion on Linux and Windows.

Most of this work starts with tracing existing runtime behavior and ends with regression coverage, cross-platform validation and review fixes.

### Agent Skills

I keep reusable Agent Skills for OpenCode and compatible coding environments in [`Aveer/skills`](https://github.com/Aveer/skills).

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

I'm building the hardware side of the Nexus ecosystem around a shared ESP32 firmware platform.

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

The goal is to give AI agents a controlled way to interact with **real-world devices and, eventually, robotics hardware**.

**C · ESP-IDF · ESP32 · ESP32-C5 · Wi-Fi · Zigbee · mDNS**

> Currently private and under active development.

---

## Selected public projects

### [OMO Slim Preset Switcher](https://github.com/Aveer/omo-slim-preset-switcher)

Small desktop utility for managing oh-my-opencode-slim presets across multiple projects.

It supports separate Global / Project / Inherit semantics, bulk project changes, OMO Slim precedence rules and JSONC-preserving atomic writes without modifying OpenCode itself.

**Python · Tkinter**

---

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

Local AI infrastructure · agentic coding · multi-agent systems · developer tooling · embedded systems · robotics · AI-to-device interfaces
