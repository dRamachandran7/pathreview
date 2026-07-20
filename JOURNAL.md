## Week 7 — Issue selection

**Issue link:** (https://github.com/ascherj/pathreview/issues/130)

**Issue title:** docker-compose.yml doesn't set memory limits for the LLM proxy service, causing OOM kills on 8GB machines

**Tier:** [ ] Tier 1  [ ] Tier 2  [x] Tier 3

**Problem summary:**
[In 3–5 sentences, in your own words: what the issue is (not a copy-paste of
the title), what is currently broken or missing, and what a successful fix
would accomplish. Naming the part of the codebase it affects is helpful context.]

The issue lies within the docker-compose.yml file. Since there is no memory limit set for the LLM proxy service, it can consume unbounded RAM, and on low memory machines, this ends up consuming memory from other service, and starts creating OOM-kills. To remedy this, we need to add a memory limit in the docker compose file, similar to the ones already being used for db, redis, and vector-db.

**Branch name:** fix/130-docker-compose-llm-proxy-memory-limits

**Setup confirmation:** [x] App runs locally at localhost:5173

**Cohort ledger:** [x] Issue added to cohort ledger