# Synthetic Examples

These examples show the judgment shape, not a required response format.

## 1. Accept a sound small plan

**Request:** “The formal Todo owner proposes a README title-only change. One reviewer will inspect the rendered Markdown, and the owner will run the repository's required check. Is more needed?”

**Advice:** “This is proportionate for a title-only change. Keep the owner and reviewer roles as stated: no additional agent or higher model tier is warranted. The rendered-Markdown inspection plus the required check is sufficient for the stated Done condition. If that heading is copied into generated documentation, include the affected output in the same inspection.”

## 2. Raise a warranted counterexample

**Request:** “Simplify a cache key from tenant plus user identifier to only the user identifier. The cache is shared, but the user identifier looks familiar across records.”

**Advice:** “This needs a counterexample before accepting the simplification: two tenants can have the same user identifier. With a user-only key, one tenant can read or overwrite the other's cached value. Retain tenant identity in the key unless a verified invariant proves the identifier is globally unique. The minimum relevant validation is a focused case with two tenants sharing one user identifier and separate expected cache entries; this example does not claim that check has run.”
