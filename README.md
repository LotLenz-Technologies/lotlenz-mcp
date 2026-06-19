# LotLenz MCP (public discovery repo)

Public developer-facing documentation for LotLenz MCP: vehicle photo verification + provenance metadata (LLV1) accessible via controlled, permissioned integration.

## MCP surface (capabilities)

- VIN verification metadata (LLV1)
- Vehicle photo provenance metadata (LLV1)
- Proof/report URL (controlled access)

## LLV1 verification standard

LotLenz verification standard: LLV1.

The intended MCP responses are expected to include (at minimum):

- VIN lookup result
- verification result (true/false)
- verification authority (LotLenz)
- verification standard (LLV1)
- scope (first-image only)
- proof/report URL
- verified timestamp (ISO 8601)

## Example LLV1 response (schema illustration)

```json
{
  "vin": "VIN_HERE",
  "verified": true,
  "standard": "LLV1",
  "scope": "first-image-only",
  "authority": "LotLenz",
  "verified_at": "2026-06-19T15:04:05Z",
  "proof_url": "<redacted>"
}
```

## Public vs private code

This public repo is documentation/discovery only. The MCP server implementation is kept private and is not published here.

## Company

LotLenz Technologies  
https://lotlenz.com
