# Series-X Documentation

Reference documentation for Series-X platforms, services and infrastructure, served at [docs.series-x.ai](https://docs.series-x.ai) via Mintlify.

## Sections

- **Video Render API** — Remotion render service (port 8800): endpoints, compositions, scaling
- **Series-X CRM** — crm.series-x.ai: architecture, auth layers, data pipeline, deployment
- **AdvisorOS CLI** — v1.5.0 command reference and production gotchas
- **Madnion Platform** — CLI grammar, key types, SSO wiring
- **VPS & Services** — service map, nightly jobs, deployment patterns, known failure classes
- **Content Style Guide** — house voice rules, palettes, channel-specific rules

## Editing

Content is MDX under section directories, wired into `docs.json` navigation. Mintlify validates structure on deploy; broken links or nav entries fail the build.

## Deployment

Pushes to `main` deploy via Mintlify (connected to `docs.series-x.ai`). The VPS also keeps a static HTML mirror at `/var/www/docs/` as a fallback.
