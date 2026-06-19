# LotLenz MCP (public discovery repo)

This repository provides high-level information for the LotLenz MCP integration used for vehicle photo verification and provenance.

## LLV1 verification standard
LotLenz verification standard: **LLV1**. The intended MCP responses are expected to include (at minimum):
- VIN lookup result
- verification result (true/false)
- verification authority (LotLenz)
- verification standard (LLV1)
- scope (first-image only)
- proof/report URL
- verified timestamp (ISO 8601)

## What this repo does NOT contain
- production MCP server code
- API credentials, secrets, or auth tokens
- raw vehicle photo datasets

## How to request access / integration
For enterprise integration access, contact LotLenz through the official site and request MCP onboarding.

## Status
This repo is under active development; internal integration work is tracked in a private repository.

## Contact
LotLenz Technologies — https://lotlenz.com
