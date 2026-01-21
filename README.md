# observability-playbook-docs
A docs-as-code sample for an observability product: clear concepts, task guides, API examples, troubleshooting, and diagrams. Built with MkDocs Material.
## Documentation Engineering Samples

A small, public, non-proprietary repository that demonstrates documentation craft and documentation-engineering practices: clear structure, docs-as-code workflows, API references, and quality controls.

## What this repository demonstrates
- **Docs-as-code**: Git-based workflow, review-friendly structure, automation-ready conventions
- **Information architecture**: topic-based structure (concept / how-to / reference / troubleshooting)
- **API documentation**: OpenAPI as the source of truth, plus a human-readable reference
- **Quality mindset**: style and consistency rules suitable for team use

## Contents (high level)
- `docs/` — Markdown content structured like a real product documentation set
- `api/` — OpenAPI examples used as “contract sources”
- `tools/` — small scripts that turn specs into human-readable docs (when applicable)
- `styles/` or `contributing/` — writing rules and conventions (style, terminology, etc.)

## How to view
- Browse the Markdown in this repo
- If published via GitHub Pages, the site mirrors the same structure

## Principles used
- Write for tasks and outcomes (not features)
- Make assumptions explicit (prereqs, auth, limits)
- Keep examples copy/pasteable
- Prefer consistent patterns over “one-off” cleverness

## License
MIT
