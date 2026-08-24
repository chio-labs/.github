# Chio Labs GitHub Policy

This repository owns organization-wide GitHub workflow policy.

`auto-merge.yml` requests squash auto-merge for ready, same-repository pull requests. Repository
rulesets and required checks remain authoritative: GitHub merges only after every required check
passes. It uses an organization-owned GitHub App so the resulting merge can trigger downstream
delivery workflows. This includes Release Please pull requests; product release workflows must use
the same App identity when creating or updating those branches so GitHub emits the pull request
events that invoke the organization workflow.

The organization ruleset applies this workflow to Chio Labs public repositories.

Draft and fork-based pull requests are intentionally excluded. A draft is handled when it becomes
ready for review. Product workflows remain responsible for release-specific validation, while this
organization workflow is the single owner of requesting auto-merge.
