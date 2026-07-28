## Week 7 — Issue selection

**Issue link:** (https://github.com/ascherj/pathreview/issues/89)

**Issue title:** API reference doc is missing the POST /profiles request body schema

**Tier:** [x] Tier 1  [ ] Tier 2  [] Tier 3

**Problem summary:**

The issue lies within docs/API.md. The doc currently documents response schemas for endpoints, but is missing request body schemas for the POST /profiles and POST /reviews endpoints. Without these, someone integrating against the API has to guess at what fields to send. To remedy this, we need to add request body schemas for both endpoints, each with field descriptions and example values.

**Branch name:** fix/89-API-reference-doc-missing-POST-profiles-schema

**Setup confirmation:** [x] App runs locally at localhost:5173

**Cohort ledger:** [x] Issue added to cohort ledger

## Issue Checklist

**Can I explain what this issue is asking for in my own words?**

Yes. The API currently is missing schemas for POST /profiles endpoint.

**Do I understand which part of the app is affected?**

Yes. The API.md doc is the root cause of the problem, and also the affected portion.

**Do I understand what "done" looks like?**

'done' means that the doc is updated with schemas and examples, following the format of other schemas in the doc.

**Is the tier a realistic match for where I am right now?**

While the fix seems pretty simple, this is my first time working with a large codebase or open source project, so it is a good fit for me.

**Can I find the relevant code?**

Yes, the relevant portion of this issue is, as mentioned, the API.md file, which has descriptions for other endpoints, but not the one described here.

**Do I understand the surrounding code well enough to change it safely?**

I understand how the other API endpoints are structured, so I do undesrstand how to best document this one.

**Have I read the relevant test file?**

Since this is a docs issue, there isn't really any test files for this.

**How many others are already working on this issue?**

There are large amount of people working on this issue, but since it is a documentation gap, I am ok with the amount of people working on it.

**Is the scope realistic for Weeks 8–9?**

Yes. All I need to do is understand the API structure and document it.


## Week 8 — Reproduction & solution planning

**Reproduction commit link:** [link to comment commit](https://github.com/dRamachandran7/pathreview/commit/2edeee5972e5cf60b9769c7448321dc74e57d057)

**Reproduction summary:**
Upon inspecting the schemas, we can see that the two endpoints described do indeed exist, and upon inspecting API.md, we can see that they are not documented. This is the gap we need to fill.

**PLAN.md link:** https://github.com/dRamachandran7/pathreview/blob/fix/89-API-reference-doc-missing-POST-profiles-schema/PLAN.md

**Walkthrough video (recommended):** [link to your Loom video, ≤2 min — recommended, not graded]

**Blockers or open questions:**
[Anything you're still uncertain about going into Week 9, or leave blank]
