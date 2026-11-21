# Copilot instructions — brand-promoter-web

Stack: Next.js + TypeScript. Product: Brand Promoter Management System.

**Functional source of truth:** sibling `../brand-promoter-docs/docs/` in the multi-root workspace. Read scope, matrix, HU spec, ADRs and DoD before implementation. If inaccessible, stop and request specific files.

Minimum backoffice: users, stores, products, assignments and reception consultation. NestJS owns business rules and permissions. No second business API in Next.js. Consume versioned OpenAPI. Prioritize basic accessibility, clear forms and admin E2E tests.

Work by HU and small PR. Inspect Git before editing. Propose a plan and await approval for broad changes. Do not assume tests were executed. Do not change contracts without documenting impact on other repositories.

## Naming and AI workflow
- Official name: Brand Promoter Management System. Technical repository prefix: `brand-promoter`.
- Use English for technical identifiers, filenames, API routes, DB objects, branches and commits; Use Spanish for business-facing specifications and UI copy. Follow the bilingual glossary and language policy in the documentation repository.
- Follow `../brand-promoter-docs/docs/process/naming-conventions.md`, `sdd-copilot.md`, `review-gates.md`, and `change-control.md`.
- Approved specs are the source of truth. Do not silently change them.
- For a completed or blocked HU, report real commands and test evidence using the implementation report template.
- Escalate cross-repository breaking contracts, schema/auth changes, new infrastructure and persistent defects.
