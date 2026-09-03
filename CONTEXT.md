# i-dot-ai/lex context
> refreshed 2026-09-03 | upstream default: main @ a31684d5fc71d070514c1d2e0f043dcad99f7a74

## Identity & policies
- upstream: i-dot-ai/lex, default branch `main`, primary language Python, English-first (yes — all docs/UI/CONTRIBUTING in English; dialect British)
- license: MIT
- CLA/DCO: none (CONTRIBUTING has no CLA/signup ask; no CLA bot observed on PRs)
- AI-assisted PR policy: unstated (no disclosure requirement)
- signed commits required: no evidence
- PR template: `.github/pull_request_template.md` (5 sections: Description / Type of Change / Related Issues / Testing / Additional Notes) — use verbatim
- external tracker: github

## Conventions (verified from merged PRs)
- branch naming: `fix/<desc>`, `feature/<desc>`, `docs/<desc>` (merged headRefNames: fix/*, feature/*, ingest-analysis); CONTRIBUTING confirms feature/|fix/|docs/
- tests: `uv run pytest tests/ -m "not integration"`; lint: `ruff format` / `ruff check` (pinned 0.14.5), pre-commit
- CI gate (`linting.yml` on PR): ruff format --check, pytest (non-integration), pip-audit; pre-commit.yml
- outside PR merges: recent merges are renovate/bot (aikido) + maintainer lmwilkigov; external human merges last seen 2025-06 (olivernormand). External open PRs pending → maintainer merge latency for outsiders is slow; docs PRs are reasonable

## Maintainer picture
- active maintainer: lmwilkigov (Liam Wilkinson); olivernormand (Oliver Normand) earlier; some bot-driven dependency churn
- recent bot PRs target deps/security; keep PRs away from dependency/security files

## Issue-area health
- mostly small; docs improvements welcomed (external docs PR #104 open)
- data pipeline is heavily documented internally

## Gap ledger (dedupe — READ FIRST, never re-pick)
- `2026-09-03` self-found docs trivial pass (README stale make targets, `--collection amendments` flag, `QDRANT_URL`→`QDRANT_HOST`, `seperate` typo, stale pdf csv/sh) — outcome: fork PR opened — lesson: doc references to nonexistent Makefile targets/scripts/env vars vs code truth

## Mined gaps (discovered, not yet attempted)
- n/a this run (single focused trivial pass only)
