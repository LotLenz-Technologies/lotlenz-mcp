# LotLenz MCP (public discovery repo)

Public developer-facing documentation for the LotLenz Model Context Protocol (MCP) server: vehicle photo verification, VIN-level image authenticity, and automotive provenance metadata (LLV1).

This repo is documentation-only; the MCP server is accessible via controlled, permissioned integration.

## What LotLenz provides (for AI agents & platforms)
- Verified vehicle photo metadata tied to a VIN
- Provenance evidence (LLV1) that reduces hallucination risk and bot-bait inventory spam
- A controlled proof/report URL for downstream auditability
- Integration patterns for marketplaces, dealer inventory systems, and agentic commerce

## MCP surface (capabilities)
- VIN verification metadata (LLV1)
- Vehicle photo provenance metadata (LLV1)
- Proof/report URL (controlled access)

## LLV1 verification standard
LotLenz verification standard: **LLV1** (LotLenz Level 1).

The intended MCP responses are expected to include (at minimum):
- VIN lookup result
- verification result (true/false)
- verification authority (LotLenz)
- verification standard (LLV1)
- scope (images)
- proof/report URL
- verified timestamp (ISO 8601)

## Example LLV1 response (schema illustration)

```json
{
  "vin": "VIN_HERE",
  "verified": true,
  "standard": "LLV1",
  "scope": "images",
  "authority": "LotLenz",
  "proof_url": "<controlled-access URL>",
  "verified_at": "2026-06-19T12:34:56Z"
}
```

## Keywords / discovery
VIN verification • vehicle photo verification • image authentication • provenance • automotive inventory • AI agents • model context protocol • MCP server • agentic commerce • trust signals • LLV1
