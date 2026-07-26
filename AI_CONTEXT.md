# AI_CONTEXT.md

# HXAI AI Context

**Version:** 1.0

**Purpose:** Shared Context for AI Coding Assistants

**Applies To:**

- GitHub Copilot
- GitHub Copilot Agent
- Kilo CLI
- Cursor
- Codex
- Claude Code
- Gemini CLI
- Future AI development tools

---

# What is HXAI?

HXAI is an ecosystem of AI-powered products focused on helping people understand knowledge through visualization, exploration, experimentation, and intelligent assistance.

HXAI is **not** a chatbot.

HXAI is a platform.

Every product inside HXAI should share the same design language, architecture, and AI infrastructure.

---

# HXAI Ecosystem

```
HXAI

│

├── HXAI Research

│ ├── Knowledge Universe

│ ├── Research Canvas

│ ├── Visualization Engine

│ ├── CAD Explorer

│ ├── Timeline Explorer

│ ├── Reports

│ ├── HXAI Labs

│ └── HXAI Copilot

│

├── Future HXAI Products

│ ├── HXAI Cloud

│ ├── HXAI API

│ ├── HXAI Studio

│ ├── HXAI SDK

│ └── Additional Products
```

Everything belongs under HXAI.

---

# Product Vision

HXAI Research is the flagship product.

Its purpose is to transform research from reading into exploration.

Instead of generating long paragraphs, HXAI should create interactive experiences that help users build understanding.

Every research session should feel like entering a digital laboratory.

---

# Current Development Stage

Current Phase

Phase 1

Foundation

The architecture has been designed.

The documentation is complete.

The implementation has begun.

---

# Completed Documentation

The following documents already exist and define the architecture.

README.md

PRODUCT_REQUIREMENTS.md

ARCHITECTURE.md

KNOWLEDGE_ENGINE.md

KNOWLEDGE_UNIVERSE.md

KNOWLEDGE_GRAVITY.md

KNOWLEDGE_PHYSICS.md

VISUALIZATION_ENGINE.md

HXAI_LABS_SPEC.md

HXAI_COPILOT.md

AGENT_ORCHESTRATOR.md

DATABASE_SCHEMA.md

API_SPEC.md

PLUGIN_SDK.md

UI_GUIDELINES.md

DESIGN_SYSTEM.md

ROADMAP.md

COPILOT_RULES.md

These documents are the source of truth.

Do not contradict them.

---

# Current Architecture

HXAI follows a modular monorepo.

```
HXAI/

apps/

packages/

docs/

assets/
```

Packages should remain independent.

Avoid coupling unrelated systems together.

---

# Current Technology Stack

Frontend

Next.js

React

TypeScript

Tailwind CSS

shadcn/ui

Framer Motion

Backend

FastAPI

Python

Database

PostgreSQL

Supabase

Authentication

Supabase Auth

Visualization

React Flow

Tldraw

Three.js

React Three Fiber

Recharts

Future

D3

Blender

OpenCascade

Godot

USD

---

# AI Architecture

HXAI supports multiple AI providers.

Never couple HXAI to one provider.

Use an abstraction layer.

Supported providers include:

OpenAI

Anthropic

Gemini

Local Models

Future providers

Switching providers should require minimal code changes.

---

# Core Systems

HXAI consists of several intelligent systems.

Knowledge Engine

Knowledge Universe

Knowledge Physics

Knowledge Gravity

Visualization Engine

HXAI Labs

HXAI Copilot

Agent Orchestrator

These systems work together.

Do not merge them into one component.

---

# Current Goal

Build the first working prototype.

Focus on:

Landing Page

Authentication

Dashboard

Research Workspace

Knowledge Universe

Visualization Engine

HXAI Copilot

HXAI Labs

Ignore advanced enterprise features until later phases.

---

# Current Priorities

Priority 1

Stable architecture

Priority 2

Clean code

Priority 3

Reusable components

Priority 4

Good documentation

Priority 5

Scalability

---

# Current UI Philosophy

Professional

Minimal

Dark Mode

Apple-level polish

Research-first

No unnecessary clutter

Visual learning over text

---

# Current Knowledge Philosophy

Knowledge should behave like a living universe.

Every topic connects to other topics.

Relationships evolve.

Nodes grow.

Knowledge expands naturally.

Avoid static trees.

---

# Current Visualization Philosophy

Do not hardcode visualizations.

The Visualization Engine decides the most appropriate representation.

Possible outputs include:

Knowledge Maps

Flowcharts

Timelines

Charts

CAD Views

Graphs

3D Models

Pictograms

Animations

Whiteboards

Reports

Future plugins should add additional visualization types.

---

# Current HXAI Labs Philosophy

HXAI Labs should never contain fixed simulations.

Instead:

Understand the topic.

Generate an experiment.

Generate controls.

Generate variables.

Run the simulation.

Explain the results.

Suggest improvements.

Every lab is dynamically generated.

---

# Current Copilot Philosophy

HXAI Copilot is an assistant.

It supports exploration.

It should not dominate the interface.

The research experience always comes first.

---

# Known Decisions

Decision

Landing page remains public.

Decision

Dashboard requires authentication.

Decision

Supabase Auth is the authentication provider.

Decision

HXAI is modular.

Decision

Visualization is dynamic.

Decision

Knowledge Universe is the gateway to research.

Decision

HXAI Labs is generated dynamically.

Decision

Research should be domain-agnostic.

Decision

Everything belongs under the HXAI ecosystem.

---

# Development Workflow

Before implementing a feature:

Read documentation.

Understand architecture.

Identify dependencies.

Implement.

Test.

Document.

Commit.

Do not skip documentation review.

---

# Coding Expectations

Strict TypeScript

Reusable components

Accessibility

Performance

Responsive layouts

Clean architecture

Meaningful commit messages

No unnecessary dependencies

---

# If Unsure

If documentation is incomplete or ambiguous:

Do not guess.

Summarize the current understanding.

Identify conflicting documents.

Ask for clarification before implementing.

---

# Long-Term Vision

HXAI is being built as a platform that allows anyone to explore, visualize, simulate, and understand knowledge.

Every architectural decision should support this long-term vision.

When making implementation choices, prefer solutions that are:

- Modular
- Scalable
- Maintainable
- Extensible
- Educational
- Consistent with the documented architecture

The goal is not simply to generate software.

The goal is to build the foundation of the world's most interactive AI-powered research platform.
