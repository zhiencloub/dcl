# DCL L1: Transport Syntax Specification 1.0.0

**Version:** 1.0.0  
**Status:** Stable · Production Ready  
**Compatibility:** Superset of MCP Core · Fully Backward Compatible

---

## 1. Introduction

DCL L1 defines a common communication syntax between AI clients (e.g., large language models) and data servers (e.g., file systems, databases, cloud storage, application APIs).

It is built on JSON-RPC 2.0 and is fully compatible with the Model Context Protocol (MCP) core specification.

---

## 2. Compatibility Statement

**All DCL 1.0 compliant implementations MUST fully support the MCP core specification.**

| Scenario | Compatibility Requirement |
|----------|---------------------------|
| MCP Client → DCL Server | Server MUST ignore unknown fields and process standard MCP requests normally |
| DCL Client → MCP Server | Client MUST NOT send DCL extension fields; only send standard MCP requests |
| DCL ↔ DCL | Full extension features supported |

---

## 3. Request Format

```json
{
  "protocol": "dcl/1.0",
  "identity": {
    "did": "did:dcl:example:user123",
    "visibility": "explicit_consent"
  },
  "query": {
    "source": "data_source_identifier",
    "intent": "retrieve",
    "parameters": {},
    "preferences": {
      "language": "en-US",
      "sort_by": "relevance"
    }
  },
  "credentials": {
    "token": "bearer_token",
    "expires": "2025-12-31T23:59:59Z",
    "revoke_endpoint": "https://provider.example/revoke"
  }
}
