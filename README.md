# TIGEM Bioinformatics Publications Index

This repository lists analysis workflows maintained by the TIGEM Bioinformatics Core.

The index is intended to be public and contains only non-sensitive metadata about analysis workflows. It does not include raw data, processed data, access keys, credentials, or unpublished analysis outputs. Some linked workflow repositories may remain private while the corresponding manuscript is under submission or peer review, and will be made public according to the publication and data-release policy.

## Landing Page

The public landing page for this index is available at:

https://bioinformatics-tigem.github.io/publications-index/

The public landing page is generated automatically from:

```text
docs/publications.json
```

The static page reads that single data file and renders the table and project cards in the browser.

The site itself is served from the `gh-pages` branch, which is generated from the contents of `docs/`.

## Add a New Workflow

To add a publication-associated workflow, add one entry to `docs/publications.json`:

```json
{
  "year": "2026",
  "topic": "single-cell RNA-seq",
  "dataset": "E-MTAB-16673",
  "pi": "De Matteis",
  "status": "In submission; workflow private until publication",
  "repository_name": "scRNAseq-OCRL-KO-kidney-organoids",
  "repository_url": "https://github.com/bioinformatics-tigem/scRNAseq-OCRL-KO-kidney-organoids"
}
```

Then commit and push. GitHub Pages will update automatically.
