LotLenz MCP (public discovery repo)

Public developer-facing documentation for LotLenz MCP: vehicle photo verification + provenance metadata (LLV1) accessible via controlled, permissioned integration.

MCP surface (capabilities):
- VIN verification metadata (LLV1)
- Vehicle photo provenance metadata (LLV1)
- Proof/report URL (controlled access)

LLV1 verification standard:
LotLenz verification standard: LLV1.
The intended MCP responses are expected to include (at minimum):
- VIN lookup result
- verification result (true/false)
- verification authority (LotLenz)
- verification standard (LLV1)
- scope (first-image only)
- proof/report URL
- verified timestamp (ISO 8601)

Example LLV1 response (schema illustration):
{
  "vin": "1FAHP2E80FG123456",
  "verified": true,
  "standard": "LLV1",
  "scope": "first-image-only",
  "authority": "LotLenz",
  "verified_at": "2026-06-19T15:04:05Z",
  "proof_url": "https://api.lotlenz.com/proof/<redacted>"
}

Public vs private:
This repo: discovery + docs
Private repo: internal MCP server code + integration details

What this repo does NOT contain:
- production MCP server code
- API credentials, secrets, or auth tokens
- raw vehicle photo datasets

How to request access / integration:
For enterprise integration access, contact LotLenz through the official site and request MCP onboarding.

Status:
This repo is under active development; internal integration work is tracked in a private repository.

Contact:
LotLenz Technologies — https://lotlenz.com
