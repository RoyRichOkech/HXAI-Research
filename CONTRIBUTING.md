# CONTRIBUTING.md

# Contributing to HXAI

Welcome to the HXAI project.

First of all, thank you for taking the time to contribute.

HXAI is an open, modular platform for interactive research, visualization, simulation, and scientific exploration.

Our goal is to build software that helps people truly understand knowledge—not just read about it.

Whether you're fixing a typo, improving performance, designing a visualization, or building a new feature, your contribution is appreciated.

---

# Code of Conduct

All contributors are expected to:

- Be respectful.
- Be constructive.
- Be collaborative.
- Welcome feedback.
- Focus on solving problems.

Personal attacks, harassment, discrimination, or hostile behavior are not tolerated.

---

# Before You Start

Before writing code, please read:

- README.md
- PRODUCT_REQUIREMENTS.md
- ARCHITECTURE.md
- DESIGN_SYSTEM.md
- UI_GUIDELINES.md
- COPILOT_RULES.md
- AI_CONTEXT.md

These documents explain how HXAI is designed and why certain architectural decisions were made.

---

# Development Philosophy

HXAI follows a few simple principles:

- Build for understanding, not just functionality.
- Keep components modular and reusable.
- Prefer simple solutions over clever ones.
- Optimize for maintainability.
- Design for scalability.
- Keep documentation synchronized with implementation.

---

# Project Structure

```
HXAI/

apps/
packages/
docs/
assets/
```

Each package should have a clear responsibility.

Avoid tightly coupling unrelated systems.

---

# Branching Strategy

Use descriptive branch names.

Examples:

feature/authentication

feature/dashboard

feature/knowledge-universe

feature/visualization-engine

feature/hxai-labs

bugfix/login-session

bugfix/typescript-errors

refactor/component-library

docs/update-readme

---

# Commit Messages

Use clear commit messages.

Examples:

feat: add Supabase authentication

feat: implement Research Canvas

fix: resolve visualization rendering bug

refactor: simplify Knowledge Engine architecture

docs: update API specification

style: improve dashboard layout

test: add unit tests for AI gateway

Avoid vague messages like:

update

fix

changes

stuff

---

# Pull Requests

Before opening a Pull Request:

- Ensure the project builds successfully.
- Resolve all TypeScript errors.
- Resolve all ESLint warnings.
- Test your changes.
- Update documentation if necessary.

Pull Requests should include:

- Summary of changes
- Why the change was made
- Screenshots (if UI changes)
- Testing notes
- Related issues

---

# Coding Standards

Use:

- TypeScript
- React
- Next.js
- Tailwind CSS

Follow:

- SOLID Principles
- Clean Architecture
- DRY
- KISS

Avoid unnecessary complexity.

---

# Component Guidelines

Components should:

- Have a single responsibility.
- Be reusable.
- Be accessible.
- Be responsive.
- Be well documented.
- Use strict typing.

Avoid creating large components with multiple unrelated responsibilities.

---

# Styling Guidelines

Follow:

DESIGN_SYSTEM.md

UI_GUIDELINES.md

Use:

- Tailwind CSS
- shadcn/ui
- Framer Motion

Avoid inline styles unless absolutely necessary.

---

# AI Development

HXAI supports multiple AI providers.

Never tightly couple features to a specific provider.

Use the AI abstraction layer.

Supported providers may include:

- OpenAI
- Anthropic
- Gemini
- Local Models

Future providers should be easy to integrate.

---

# Knowledge System

The following systems are independent modules:

- Knowledge Engine
- Knowledge Universe
- Knowledge Gravity
- Knowledge Physics
- Visualization Engine
- HXAI Labs
- HXAI Copilot
- Agent Orchestrator

Do not merge these systems together.

Each has a distinct responsibility.

---

# Testing

All new features should be tested.

Where practical, include:

- Unit tests
- Integration tests
- End-to-end tests

Test both successful and failure scenarios.

---

# Documentation

If a change affects architecture, APIs, workflows, or user experience:

Update the relevant documentation.

Documentation should remain the source of truth.

---

# Performance

Consider performance before introducing dependencies.

Prefer:

- Lazy loading
- Code splitting
- Memoization where appropriate
- Efficient rendering
- Optimized assets

Avoid premature optimization, but don't ignore obvious bottlenecks.

---

# Accessibility

HXAI aims to meet WCAG 2.2 AA standards.

Ensure:

- Keyboard navigation
- Screen reader compatibility
- High contrast support
- Reduced motion support
- Responsive layouts

Accessibility is a core feature, not an afterthought.

---

# Security

Never commit:

- API keys
- Secrets
- Database credentials
- Private tokens
- Environment files

Validate all user input.

Follow secure authentication practices.

Report security issues responsibly.

---

# Issues

When reporting an issue, include:

- Clear description
- Steps to reproduce
- Expected behavior
- Actual behavior
- Screenshots (if applicable)
- Environment information

Good bug reports help everyone.

---

# Feature Requests

Feature requests should explain:

- The problem being solved.
- The proposed solution.
- Alternative approaches considered.
- How it aligns with HXAI's vision.

Not every feature request will be accepted.

The long-term architecture takes priority over short-term convenience.

---

# Recognition

Every contributor helps shape HXAI.

Whether your contribution is one line of documentation or an entirely new subsystem, it is valued.

Thank you for helping build HXAI.

---

# Final Principle

HXAI is more than software.

It is an effort to redefine how people learn, explore, and understand knowledge.

Every contribution should move the project closer to that vision.

Welcome to HXAI.
