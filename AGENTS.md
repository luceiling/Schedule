# AGENTS.md

## Purpose

This file defines how humans and coding agents should work in this project to safely experiment with DayPilot, build proofs of concept, and implement production-ready changes.

## Edition and Boundaries

- Current edition: `pro`
- Target: `javascript`
- Component focus: `scheduler`
- Project alias: `daypilot-project`
- DayPilot feature availability differs between Lite and Pro. Verify compatibility before implementation.

## Trusted Sources (Priority Order)

Use sources in this order:
1. Local type definitions first (API shape and availability checks):
- `js/daypilot/daypilot-all.min.d.ts`
- `Bundled with this project template.`
2. Official docs, API reference, tutorials, and demos:
- `https://doc.daypilot.org/`
- `https://api.daypilot.org/`
- `https://javascript.daypilot.org/`
- `https://code.daypilot.org/`
- `https://javascript.daypilot.org/demo/`
- `https://javascript.daypilot.org/demo/lite/`
- `https://github.com/DayPilotCode`
3. Edition confirmation:
- `https://javascript.daypilot.org/feature-matrix/`
4. Supporting context only:
- `https://forums.daypilot.org/`

Forum content may be outdated. Treat it as supportive context and verify any advice against official docs/API and current typings.

## Repository Working Rules

- Keep changes scoped and avoid unrelated edits.
- Prefer source-backed implementation decisions.
- If behavior/config changes, update docs in the project.
- Do not run destructive git commands unless explicitly requested.

## Common Workflows

### PoC experiment flow
1. Define one clear goal and target component behavior.
2. Confirm API availability in typings and feature matrix.
3. Implement the smallest working change.
4. Capture result, constraints, and next step.

### Implementation/hardening flow
1. Identify affected files and expected behavior.
2. Validate API and edition availability from trusted sources.
3. Implement with focused changes and run project validation.
4. Summarize files changed, tests run, and residual risk.

### Edition compatibility check flow
1. Check local lite/pro typings for candidate API.
2. Validate against `feature-matrix`.
3. If unavailable in current edition, document fallback or upgrade path.

## Validation Checklist

- Build/test commands from project README were executed (or limitation documented).
- Visual/behavioral outcome matches intent.
- Edition compatibility verified and noted.
- Source references captured for non-obvious API decisions.

## Escalation

If a feature cannot be fully configured in the online builder, continue in this project using source-backed implementation and record assumptions/limits.


## Pro Notes

- Pro-only features are allowed but still require compatibility verification.
