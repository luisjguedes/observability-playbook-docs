# Observability Playbook Docs

Use this repo to document incident detection and troubleshooting guidance in a consistent, Microsoft-style voice.

## What’s included

- A playbook structure for troubleshooting topics
- Style rules enforced with Vale
- A docs site build (MkDocs Material)

## How this repo works

!!! info "From draft to published docs"
    This repo treats documentation like code: changes are reviewed, checked for style, built, and deployed automatically.

    ```mermaid
    flowchart LR
      A["Write docs<br/>(Markdown)"] --> B["Open PR<br/>(review)"]
      B --> C["Style checks<br/>(Vale + MS style)"]
      C --> D["Build site<br/>(MkDocs Material)"]
      D --> E["Deploy<br/>(GitHub Pages)"]
      E --> F["Published site"]
    ```
