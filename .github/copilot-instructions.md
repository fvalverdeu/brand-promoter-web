# Copilot instructions — brand-promoter-web

Stack: Next.js + TypeScript. Product: Brand Promoter Management System.

**Functional source of truth:** sibling `../brand-promoter-docs/docs/` in the multi-root workspace. Read scope, matrix, HU spec, ADRs and DoD before implementation. If inaccessible, stop and request specific files.

Minimum backoffice: users, stores, products, assignments and reception consultation. NestJS owns business rules and permissions. No second business API in Next.js. Consume versioned OpenAPI. Prioritize basic accessibility, clear forms and admin E2E tests.

Work by HU and small PR. Inspect Git before editing. Plan routine authorized work autonomously; obtain approval for changes outside the autonomy policy. Do not assume tests were executed. Do not change contracts without documenting impact on other repositories.

## Naming and AI workflow
- Official name: Brand Promoter Management System. Technical repository prefix: `brand-promoter`.
- Use English for technical identifiers, filenames, API routes, DB objects, branches and commits; Use Spanish for business-facing specifications and UI copy. Follow the bilingual glossary and language policy in the documentation repository.
- Follow `../brand-promoter-docs/docs/process/naming-conventions.md`, `sdd-copilot.md`, `review-gates.md`, and `change-control.md`.
- Approved specs are the source of truth. Do not silently change them.
- For each completed or blocked HU, persist an English implementation record using the template; do not require a chat handoff.
- Escalate cross-repository breaking contracts, schema/auth changes, new infrastructure and persistent defects.

## Autonomous workflow (v0.4.0)
Read the canonical `brand-promoter-docs/docs/process/autonomy-policy.md`, `review-package-policy.md`, `review-gates.md`, `language-policy.md` and `sdd-copilot.md` before work. Continue authorized ready items without per-HU prompts. At gates or escalation, create an external ZIP with Spanish report and Git evidence using `brand-promoter-docs/.github/skills/generate-review-package/SKILL.md` (read directly if not discoverable). Stop for approval. Never export secrets or alter the real Git index for evidence. No implementation before Gate 1 approval.
