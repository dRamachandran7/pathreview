## Week 7 — Issue selection

**Issue link:** (https://github.com/ascherj/pathreview/issues/89)

**Issue title:** API reference doc is missing the POST /profiles request body schema

**Tier:** [x] Tier 1  [ ] Tier 2  [] Tier 3

**Problem summary:**

The issue lies within docs/API.md. The doc currently documents response schemas for endpoints, but is missing request body schemas for the POST /profiles and POST /reviews endpoints. Without these, someone integrating against the API has to guess at what fields to send. To remedy this, we need to add request body schemas for both endpoints, each with field descriptions and example values.

**Branch name:** fix/130-docker-compose-llm-proxy-memory-limits

**Setup confirmation:** [x] App runs locally at localhost:5173

**Cohort ledger:** [x] Issue added to cohort ledger