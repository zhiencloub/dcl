# DCL (Data Commons Language)

**Version 1.0.0 · Official Release**

An open, neutral, and extensible data access protocol for AI.  
Fully compatible with [Model Context Protocol (MCP)](https://github.com/anthropic/mcp).

---

## Overview

DCL defines a universal communication syntax between Large Language Models (clients) and data sources (servers) — including file systems, databases, cloud storage, and application APIs.

It is designed with three core objectives:

- **Compatibility First** — DCL 1.0 is a superset of MCP. Every DCL implementation fully supports standard MCP.
- **Optional by Design** — All DCL extensions are optional and never break existing MCP ecosystems.
- **Transparency by Default** — DCL requires human-readable explanations for ranking logic and permission summaries.

---

## Protocol Stack

| Layer | Name | Status | Description |
|-------|------|--------|-------------|
| L1 | Transport Syntax | **1.0.0 Stable** | Request/response format, authentication, metadata |
| L2 | Identity Syntax | Draft | Decentralized identity and cross-domain migration |
| L3 | License Syntax | Planning | Data usage condition declaration |

---

## Quick Start

### 1. Read the Specification
Full protocol specification: [`PROTOCOL.md`](./PROTOCOL.md)

### 2. Reference Implementations
- Python (in progress)
- TypeScript (in progress)

### 3. Community & Contributions
- Issues & Discussions: GitHub Issues
- Contribution Guide: [`CONTRIBUTING.md`](./CONTRIBUTING.md)

---

## Repository

| Role | Platform | URL |
|------|----------|-----|
| **Primary** | GitHub | https://github.com/zhiencloub/dcl |
| Mirror (China) | Gitee | https://gitee.com/dcl-org/dcl |

---

## Language Versions

| Language | File |
|----------|------|
| English | [README.md](./README.md) |
| Chinese (Simplified) | [README.zh-CN.md](../README.zh-CN.md) |

---

## License

- **Code**: MIT License
- **Documentation**: CC BY 4.0
- **Protocol Specification**: Public Domain

---

## Maintainers

DCL is maintained by an open-source community. The initial proposal was contributed by developers from China, with global contributors and adopters welcome.
