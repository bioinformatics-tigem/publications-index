---
layout: default
title: Reproducible Analysis Workflows
---

# TIGEM Bioinformatics Core: Reproducible Analysis Workflows

The TIGEM Bioinformatics Core maintains curated analysis workflows associated with scientific publications and collaborative research projects.

Our goal is to support reproducibility, transparency, and long-term accessibility of computational analyses by providing documented code, configuration files, software requirements, metadata templates, and links to public datasets whenever possible.

## Mission

We aim to make bioinformatics analyses easier to inspect, rerun, and reuse. Each workflow is organized to separate code, configuration, sample metadata, and data access instructions.

## What This Index Contains

This public index contains non-sensitive metadata about analysis workflows maintained by the TIGEM Bioinformatics Core. It does not include raw data, processed data, access keys, credentials, or unpublished analysis outputs.

Some workflow repositories may remain private while the corresponding manuscript is under submission or peer review, and will be made public according to publication and data-release policies.

## Workflow Standards

Whenever possible, each workflow includes:

- documented notebooks or scripts
- software requirements or environment files
- configuration files for paths and parameters
- sample metadata templates
- public dataset accession numbers
- instructions to regenerate key input objects
- notes on data access and expected outputs

## Publications And Workflows

| Year | Topic | Dataset | PI | Status | Repository |
|---|---|---|---|---|---|
{% for pub in site.data.publications.publications %}
| {{ pub.year }} | {{ pub.topic }} | {{ pub.dataset }} | {{ pub.pi }} | {{ pub.status }} | [{{ pub.repository_name }}]({{ pub.repository_url }}) |
{% endfor %}

## Workflow Cards

{% for pub in site.data.publications.publications %}
### {{ pub.repository_name }}

- **Year:** {{ pub.year }}
- **Topic:** {{ pub.topic }}
- **Dataset:** {{ pub.dataset }}
- **PI:** {{ pub.pi }}
- **Status:** {{ pub.status }}
- **Repository:** [{{ pub.repository_name }}]({{ pub.repository_url }})

{% endfor %}

## Contact

For questions about these workflows, contact the TIGEM Bioinformatics Core at `bicore@tigem.it`.
