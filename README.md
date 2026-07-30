# Leland

Leland is a marketplace for ambitious people to access the coaching, classes, and community they need to reach career and educational goals. It connects individuals with vetted 1-on-1 coaches across MBA and college admissions, management consulting, investment banking, private equity, product management, law, medicine, and executive and career development, and sells structured live programs, bootcamps, and test prep for the GMAT, GRE, LSAT, MCAT, SAT, and ACT. Leland+ is a subscription content library of video guides, essay and resume examples, templates, and expert-built AI tools. For organizations Leland offers AI-native talent training, agentic workflow deployment, recruiting, and outplacement.

Website: https://www.joinleland.com — Backed by: forerunner-ventures

## API surface

Leland publishes **no public API, developer portal, or API documentation** as of 2026-07-19. Enrichment probes returned 404 or no DNS for `api.`, `developers.`, `docs.`, `status.`, and `trust.` subdomains, for `/api`, `/developers`, `/api-docs`, and `/llms.txt`, and for the full `/.well-known/` discovery surface. Artifacts in this repo are therefore limited to identity, a generated `llms.txt`, and probed security posture — nothing has been fabricated.

## Artifacts

- `security/leland-domain-security.yml` — probed TLS/DNS posture (TLS 1.3, SPF and DMARC present, no HSTS, no DNSSEC, no CAA).
- `well-known/leland-well-known.yml` — negative probe record for the `/.well-known/` surface.
- `llms/leland-llms.txt` — generated from this catalog entry.
