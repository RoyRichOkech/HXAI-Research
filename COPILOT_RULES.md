# COPILOT_RULES.md

# HXAI Development Rules

**Version:** 1.0

**Applies To:**
- GitHub Copilot
- GitHub Copilot Agent
- Kilo CLI
- Codex
- Cursor
- Claude Code
- Any future AI coding assistant

---

# Purpose

These rules define the engineering principles of HXAI.

Every AI assistant contributing code to this repository MUST follow these rules.

If documentation conflicts with generated code, **the documentation is the source of truth**.

Never make architectural decisions without consulting the documentation.

---

# Read Before Coding

Before implementing any feature, always read the relevant documents inside `/docs`.

Minimum required documents:

- README.md
- PRODUCT_REQUIREMENTS.md
- ARCHITECTURE.md
- DESIGN_SYSTEM.md
- UI_GUIDELINES.md

Additional documents depending on the feature:

Research
→ KNOWLEDGE_ENGINE.md

Knowledge Graph
→ KNOWLEDGE_UNIVERSE.md

Visualization
→ VISUALIZATION_ENGINE.md

Labs
→ HXAI_LABS_SPEC.md

Copilot
→ HXAI_COPILOT.md

Database
→ DATABASE_SCHEMA.md

API
→ API_SPEC.md

Plugins
→ PLUGIN_SDK.md

Roadmap
→ ROADMAP.md

---

# Product Philosophy

HXAI is NOT a chatbot.

HXAI is an interactive research platform.

Always prioritize:

Understanding

Visualization

Exploration

Experimentation

Discovery

Do not build interfaces that resemble ChatGPT.

---

# Architecture

Never place everything inside one application.

Follow the modular architecture.

HXAI/

apps/

packages/

docs/

assets/

Each package must have one responsibility.

---

# Coding Principles

Always follow:

SOLID

Clean Architecture

DRY

KISS

Composition over inheritance

Reusable components

Separation of concerns

Strict TypeScript

Accessibility

Performance

Never sacrifice architecture for convenience.

---

# TypeScript Rules

Always enable strict mode.

Avoid "any".

Use interfaces and types appropriately.

Use generics where useful.

Export reusable types.

Never ignore compiler errors.

The project should compile without warnings.

---

# React Rules

Prefer Server Components when appropriate.

Use Client Components only when necessary.

Keep components small.

Each component should have a single responsibility.

Do not create extremely large files.

Prefer composition.

Use reusable hooks.

---

# Styling Rules

Use only:

Tailwind CSS

shadcn/ui

Framer Motion

Follow DESIGN_SYSTEM.md.

Never hardcode repeated styles.

Create reusable UI primitives.

---

# Research Rules

Every research topic should answer:

What is it?

How does it work?

Why does it work?

How can it be explored?

Can it be simulated?

Never return text alone when a visualization would improve understanding.

---

# Knowledge Universe Rules

Knowledge Universe is the central navigation system.

It is NOT just a graph.

It is the intelligent gateway that decides:

Which AI agents should participate

Which visualizations should be created

Which simulations should be generated

Which reports should be produced

Everything begins inside the Knowledge Universe.

---

# Knowledge Gravity Rules

Knowledge Gravity determines:

importance

relationships

learning order

research priority

Do not hardcode relationships.

Relationships should be generated dynamically.

---

# Knowledge Physics Rules

Knowledge should behave like a living system.

Nodes evolve.

Relationships change.

Knowledge grows.

Connections strengthen over time.

Avoid static graphs.

---

# Visualization Rules

Never hardcode visualization types.

Instead:

Analyze the topic.

Choose the best visualization.

Possible outputs:

Flowcharts

Knowledge Maps

Timelines

Charts

Graphs

CAD Views

3D Models

Pictograms

Animations

Research Canvas

Allow future visualization plugins.

---

# HXAI Labs Rules

HXAI Labs must never be hardcoded.

Never create:

Battery Simulator

Rocket Simulator

Robot Simulator

as fixed pages.

Instead:

Understand the research topic.

Generate a dynamic experiment.

Create controls.

Generate variables.

Run simulations.

Explain results.

Every lab is created dynamically.

---

# HXAI Copilot Rules

HXAI Copilot assists the user.

It never replaces exploration.

The Copilot understands:

Current research

Knowledge node

Simulation

Visualization

Selected component

User goals

The Copilot should:

Explain

Teach

Suggest

Debug

Compare

Summarize

Never interrupt users unnecessarily.

---

# AI Rules

Never tie HXAI to one provider.

Always use an AI abstraction layer.

Supported providers may include:

OpenAI

Anthropic

Gemini

Local Models

Future Providers

Changing providers should require minimal code changes.

---

# Authentication Rules

Use Supabase Auth.

Do not use Clerk.

Use PostgreSQL.

Protect private routes.

Landing Page must remain public.

---

# Data Rules

Never hardcode research domains.

The system should support:

Engineering

Medicine

Physics

Biology

Chemistry

Agriculture

Space

Architecture

Mathematics

Future domains

Design everything to be domain-agnostic.

---

# API Rules

Follow API_SPEC.md.

Do not invent endpoints.

Keep APIs RESTful.

Version APIs.

Validate inputs.

Return consistent responses.

---

# Database Rules

Follow DATABASE_SCHEMA.md.

Never duplicate data.

Use relationships.

Support future scaling.

---

# Plugin Rules

Everything should be extendable.

Future developers should be able to add:

Research domains

Labs

AI agents

Visualizations

Reports

Knowledge providers

without modifying HXAI Core.

---

# UI Rules

Follow UI_GUIDELINES.md.

Dark Mode first.

Professional.

Minimal.

Research-focused.

Apple-level polish.

Avoid clutter.

---

# Performance Rules

Prefer lazy loading.

Avoid unnecessary re-renders.

Optimize large visualizations.

Use virtualization where needed.

Support large knowledge graphs.

---

# Accessibility Rules

Keyboard navigation.

Screen reader support.

High contrast.

Reduced motion.

Responsive layouts.

WCAG compliance.

---

# Documentation Rules

Every major feature should include documentation.

Public APIs require comments.

Complex algorithms should be explained.

Keep documentation synchronized with implementation.

---

# Before Every Commit

Verify:

✓ Builds successfully

✓ No TypeScript errors

✓ No ESLint errors

✓ Architecture respected

✓ Documentation still accurate

✓ Components reusable

✓ Performance acceptable

✓ Accessibility maintained

---

# If Documentation Is Unclear

Never guess.

Summarize your understanding.

Identify the ambiguity.

Ask for clarification before implementing.

---

# Long-Term Vision

HXAI is not just another AI application.

It is a platform for interactive scientific discovery.

Every line of code should move HXAI closer to becoming the world's leading environment for research, visualization, experimentation, and understanding.

When in doubt, choose the solution that is:

More modular.

More reusable.

More scalable.

More educational.

More maintainable.

More aligned with the HXAI vision.
