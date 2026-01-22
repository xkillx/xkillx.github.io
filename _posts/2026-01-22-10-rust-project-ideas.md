---
title: 10 Rust Project Ideas to Level Up Your Skills
---

Learning Rust sticks best when you ship small, purposeful projects. Below are ten scoped ideas you can execute sequentially or pick à la carte depending on whether you enjoy CLI tooling, backend services, or systems tinkering.

![Rust project ideas](/images/rust-project-ideas.jpg)

## 1. CLI To-Do App

**Scope:** Manage tasks from the terminal—add, list, edit, delete, and persist to JSON/TOML or SQLite using `clap`/`structopt`. \
**Skill boost:** Strengthens I/O ergonomics, argument parsing, and error handling on a lightweight codebase.

## 2. Web Scraper

**Scope:** Fetch pages with `reqwest`, parse DOM via `scraper`, and export structured data to CSV or a database. \
**Skill boost:** Teaches HTTP clients, resilient parsing, and rate limiting for polite automation.

## 3. Simple Chat Server

**Scope:** Build a TCP or WebSocket chat with basic rooms and a plaintext protocol atop `tokio`. \
**Skill boost:** Provides hands-on ownership/lifetime practice inside concurrent networking code.

## 4. File Encryption Tool

**Scope:** CLI that encrypts/decrypts files via AES, deriving keys from passwords or passphrases. \
**Skill boost:** Reinforces secure file I/O patterns, cryptographic APIs, and meticulous Result handling.

## 5. URL Shortener Service

**Scope:** Build REST endpoints that mint short codes, store mappings in SQLite/Postgres, and redirect hits. \
**Skill boost:** Covers routing (Actix/Axum), persistence, and RESTful design on a compact backend.

## 6. Minimal REST API

**Scope:** CRUD service (notes, bookmarks, etc.) with JSON I/O, validation, and API keys. \
**Skill boost:** Deepens understanding of middleware, data modeling, and ORMs like `sqlx` or `diesel`.

## 7. Static Site Generator

**Scope:** Parse Markdown plus templates (e.g., `tera`) to output a themed static site with metadata config. \
**Skill boost:** Exercises file traversal, templating, and cohesive CLI UX design.

## 8. Markdown → HTML Converter

**Scope:** Implement a parser for headings, lists, and code blocks, either as a CLI or reusable library. \
**Skill boost:** Hones parsing strategies, string manipulation, and crate API design.

## 9. Basic HTTP Server

**Scope:** Serve static files and a couple of dynamic routes using `std::net` or a thin HTTP crate. \
**Skill boost:** Illuminates TCP primitives, manual HTTP handling, and async I/O fundamentals.

## 10. Blockchain Prototype

**Scope:** Model blocks with hashes, simple proof-of-work/stake, and a file-backed or peer-to-peer ledger. \
**Skill boost:** Explores data-structure integrity, hashing, and serialization in a safety-critical domain.
