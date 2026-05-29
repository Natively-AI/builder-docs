# Natively documentation

## About this project

- Product documentation for [Natively](https://nativelyai.com), built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links before publishing

## Terminology

| Term | Usage |
|------|--------|
| **Natively** | Product name — a software factory, not "Conductor" in user-facing docs |
| **Software factory** | Core positioning — agents produce software on a production line |
| **Workspace** | The factory floor — team, billing, projects, and members |
| **Project** | One product run through the factory |
| **Agent** | A specialist worker (Product Architect, Builder, Task Planner, Feedback) |
| **Credits** | Fuel for agent work — pay for output, not headcount |
| **Publish** | Ship factory output to a live URL on `*.nativelyai.app` |

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Link to the live app at `https://nativelyai.com` when referencing in-product actions

## Content boundaries

- Document user-facing product behavior only
- Do not document internal admin tooling, infra, or unreleased features
- Skip troubleshooting pages for now — route users to **Support** instead
- Keep plan details aligned with the in-app pricing page

## Editing workflow

1. Edit the relevant `.mdx` file
2. Run `mint dev` locally to preview
3. Open a PR — Mintlify deploys a preview URL automatically when connected to GitHub
