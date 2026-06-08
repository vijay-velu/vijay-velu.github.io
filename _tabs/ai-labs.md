---
icon: fas fa-brain
title: AI Labs
order: 6
permalink: /ai-labs/
---

Building and running AI systems — local-first inference, autonomous agents, and cloud AI tooling.

---

## Local AI Stack

Full offline inference stack. No cloud dependency for day-to-day tasks.

```
Paperclip Agents (localhost:3100)
  └── OpenCode CLI
        ├── Ollama (localhost:11434) — qwen2.5-coder:7b (GPU, GTX 1660 Ti)
        └── LM Studio (localhost:1234) — gemma-4-12b-qat, qwen3.6-27b (CPU/RAM)

Open WebUI (localhost:13000) — interactive chat, RAG, document Q&A
```

| Service | Model | Use |
|---|---|---|
| Ollama | qwen2.5-coder:7b | GPU-accelerated coding, refactors, fast inference |
| LM Studio | gemma-4-12b-qat | Planning, reasoning, multi-step tasks |
| LM Studio | qwen3.6-27b | Complex reasoning (CPU, slow) |
| LM Studio | gemma-4-e4b | Fast small tasks |
| Paperclip | CEO + CTO agents | Autonomous task execution via opencode_local adapter |

---

## Claude Agents

Custom agent configurations built in Claude.ai for real workflows. Each agent has a focused system prompt, the right model, and MCP server connections where needed.

| Agent | Model | Purpose |
|---|---|---|
| 🔍 Deep Researcher | claude-sonnet-4-6 | Multi-step web research with source synthesis and citations |
| 📊 Data Analyst | claude-sonnet-4-6 | Load, explore, and visualize data; build reports from datasets |
| 🚨 Incident Commander | claude-opus-4-6 | Triage alerts, incident triage, structured response |
| ⚙️ Structured Extractor | claude-sonnet-4-6 | Parse unstructured text into typed JSON schemas |

---

## Claude Code

Using **Claude Code CLI** as a daily development tool. Every app in [Vee Labs](/vee-labs/) — BreachGuard and ACServiceApp — was built with Claude Code handling architecture, refactors, security hardening, and CI/CD setup.

**Tooling in use:**
- Claude Code CLI + VS Code extension
- Custom MCP server configurations
- Project-level `CLAUDE.md` files for persistent context
- Hooks for automated post-edit checks
- Subagents for parallel research and code review
- Auto-memory system across all sessions

---

## Google AI

Certified in Google's AI agent track. Exploring agentic system design with Gemini and Vertex AI.

**Certifications:**
- **Agent Assist & Gen AI** — Google
- **Build AI Agents** — Google

**Tools & platforms:** Gemini · Google AI Studio · Vertex AI · Google Cloud

---

## Prompt Engineering

A working collection of prompts and agent configurations for research, writing, analysis, and decision support — built from real use, not theory.

**Approaches explored:**
- Multi-source synthesis and conflict resolution
- Devil's advocate and steelmanning for decision review
- Structured extraction with strict JSON schema adherence
- Persona-based coaching (fitness, language, negotiation)
- Agentic workflows with tool use and MCP integrations
- Local LLM evaluation and model selection for specific task types
