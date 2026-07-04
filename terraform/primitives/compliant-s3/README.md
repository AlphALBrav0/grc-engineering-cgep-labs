# Compliant S3 Primitive (Lab 2.3)

A single S3 bucket, plus its access-log bucket, built compliant by construction.
Enforces five NIST 800-53 controls in code:

- **SC-28** — encryption at rest (AES-256)
- **AC-3** — full public-access block (all four flags)
- **AU-3 / AU-6** — server access logging to a dedicated log bucket
- **CM-6** — required compliance tags + versioning

Evidence for these controls is captured as machine-readable JSON in
`evidence/lab-2-3/`.