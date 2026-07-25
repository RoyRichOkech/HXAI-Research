# DATABASE_SCHEMA.md

# HXAI Database Schema

**Version:** 1.0 Alpha

**Status:** Core Backend Architecture

**Priority:** ⭐⭐⭐⭐⭐

**Parent Product:** HXAI Research

---

# Executive Summary

The HXAI Database is designed to support a living research ecosystem rather than a traditional application.

Instead of storing only users and documents, the database stores knowledge, relationships, simulations, AI sessions, visualizations, research reports, plugins, and collaborative workspaces.

The architecture is modular, scalable, and designed for millions of interconnected knowledge objects.

---

# Design Philosophy

The database should answer three questions efficiently:

1. Who is the user?
2. What knowledge are they exploring?
3. How is everything connected?

Everything else builds upon those three foundations.

---

# Database Technologies

Primary Database

• PostgreSQL (Supabase)

Why

• Relational integrity

• JSON support

• Extensions

• Scalability

• Full-text search

• Row-Level Security (RLS)

---

Vector Database

Purpose

Semantic search

Research similarity

Knowledge embeddings

Future AI memory

Recommended

pgvector

or

Pinecone (future)

---

Object Storage

Supabase Storage

Stores

Images

Research PDFs

CAD Models

3D Assets

Videos

Generated Reports

Simulation Files

User Uploads

---

# Database Overview

```
Users

↓

Projects

↓

Research Sessions

↓

Knowledge Objects

↓

Visualizations

↓

HXAI Labs

↓

Reports

↓

Saved Research

↓

Collaboration
```

---

# Core Tables

## Users

Stores account information.

Fields

id

email

username

display_name

avatar

bio

role

created_at

updated_at

---

## User Preferences

Stores personalization.

Fields

theme

language

learning_level

preferred_domains

favorite_topics

notification_settings

layout_preferences

---

## Projects

A project groups related research together.

Example

Reusable Rocket

AI Robot

Battery Research

Fields

id

owner_id

title

description

visibility

created_at

updated_at

---

## Research Sessions

Every search creates a research session.

Stores

Current topic

Research history

Current workspace

Current agents

Open panels

Simulation state

Canvas state

Progress

---

## Knowledge Objects

The heart of HXAI.

Every concept becomes a Knowledge Object.

Examples

GPU

Mars

Photosynthesis

DNA

Fields

id

title

slug

description

domain

difficulty

summary

created_at

updated_at

---

## Knowledge Relationships

Connects knowledge objects.

Example

GPU

↓

Machine Learning

↓

CUDA

↓

Tensor Core

Relationship Types

Depends On

Contains

Uses

Invented By

Inspired By

Related To

Supersedes

Competes With

---

## Knowledge Physics

Stores dynamic values.

Fields

gravity_score

energy_score

resonance_score

entropy_score

bridge_score

evolution_stage

These values are continuously updated.

---

## Visualizations

Stores generated visual assets.

Types

Knowledge Map

Flowchart

Timeline

Graph

Diagram

CAD View

Animation

Whiteboard

3D Scene

Each visualization links back to a Knowledge Object.

---

## Research Canvas

Stores canvas state.

Zoom level

Node positions

Annotations

Bookmarks

Layers

Connections

Shared collaborators

---

## HXAI Labs

Stores simulation information.

Example

Simulation

Variables

Current values

Results

Snapshots

Experiment history

Performance metrics

---

## HXAI Copilot Conversations

Stores AI interactions.

Messages

Context

Current workspace

Referenced concepts

Current simulation

Agent responses

Summaries

---

## Agent Sessions

Tracks AI agent activity.

Agent Name

Current Task

Status

Duration

Confidence

Result

Sources Used

---

## Reports

Stores generated reports.

Executive Summary

Visualizations

Research Papers

References

Export Status

Version History

---

## Research Papers

Metadata only.

Stores

Title

Authors

DOI

Publisher

Publication Date

Citation Count

Abstract

Source URL

Knowledge Objects Linked

---

## Bookmarks

Allows users to save:

Research

Labs

Knowledge Maps

Visualizations

Reports

Experiments

---

## Notes

User-created notes.

Supports

Markdown

Images

Equations

Drawings

Attachments

Linked Concepts

---

## Files

Stores uploaded assets.

Examples

PDF

CSV

Images

CAD

Videos

Research Data

---

## Plugins

Future plugin ecosystem.

Fields

Plugin Name

Developer

Version

Permissions

Capabilities

Enabled

---

## Organizations

Future collaboration.

Universities

Companies

Research Labs

Schools

Teams

---

## Shared Workspaces

Multiple users.

Permissions

Owner

Editor

Viewer

Guest

---

# Relationships

```
User

↓

Project

↓

Research Session

↓

Knowledge Object

↓

Visualization

↓

Simulation

↓

Report

↓

Export
```

---

# Search Architecture

Supports

Keyword Search

↓

Semantic Search

↓

Knowledge Search

↓

Relationship Search

↓

Research Paper Search

↓

Project Search

↓

Natural Language Search

---

# Caching

Frequently accessed knowledge should be cached.

Examples

Popular Topics

AI

GPU

CPU

Physics

Mathematics

Frequently viewed visualizations

Research papers

Knowledge maps

---

# Security

Every user owns their data.

Implement

Row-Level Security

JWT Authentication

Encrypted Storage

Role-Based Access

Audit Logs

Version History

---

# Performance

The database should support:

Millions of Knowledge Objects

Millions of Relationships

Millions of Visualizations

Millions of Research Sessions

Without redesigning the architecture.

---

# Future Expansion

Future tables may include:

Knowledge Marketplace

AI Models

Simulation Marketplace

Research Challenges

Patents

Scientific Datasets

Public APIs

University Courses

Achievements

Community Contributions

No redesign should be required.

---

# Long-Term Vision

The HXAI Database is not merely a storage system.

It is the foundation of a living knowledge ecosystem.

Every concept, visualization, experiment, report, AI interaction, and research session is interconnected through a scalable architecture that allows HXAI Research to grow from a personal research assistant into a global scientific knowledge platform.

The schema is designed to evolve alongside the Knowledge Universe, supporting future discoveries, new domains, collaborative research, and increasingly intelligent AI systems without requiring fundamental architectural changes.
