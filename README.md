# Chio Labs GitHub Policy

This repository owns organization-wide GitHub workflow policy.

`auto-merge.yml` requests squash auto-merge for ready, same-repository pull requests. Repository
rulesets and required checks remain authoritative: GitHub merges only after every required check
passes. It uses an organization-owned GitHub App so the resulting merge can trigger downstream
delivery workflows. Release Please branches are excluded because each product's release workflow
validates those pull requests and requests auto-merge itself with the same App identity.

The organization ruleset applies this workflow to Chio Labs public repositories.

Draft and fork-based pull requests are intentionally excluded. A draft is handled when it becomes
ready for review. Release Please pull requests remain owned by each product's release workflow.
