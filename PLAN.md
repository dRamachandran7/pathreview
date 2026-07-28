## Solution plan

**Issue:** https://github.com/ascherj/pathreview/issues/89

### Understand
The issue here is that there are missing response schema documentations for POST /profiles and POST /reviews in API.md

### Map
The main file involved here is API.md, however in a broader sense, api/routes/profiles.py and api/schemas/review.py are the source of truth for the documentation.

### Plan

1. Investigate profiles.py and review.py, understand structure
2. Record the response schema in API.md
3. Create an example in API.md

### Inputs & outputs
There aren't really any inputs or outputs since this issue is strictly documentation.

### Risks & unknowns
The only real risk here is incorrect documentation, which won't affect any other file, but might create some confusion for someone reading through the codebase. For example, a new developer might be unclear on how exactly the API responds, and won't have a concrete documentation to use to clarify.

### Edge cases
When documenting examples, we should make sure that we have a representative idea of the response. We should also make sure that we explain each field in the documentation, so that all edge cases are documented. For instance, we should note that the github profile, resume, and portfolio fields can all possibly be None.