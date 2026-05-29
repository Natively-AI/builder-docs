# Native.Builder documentation

## About this project

- Product documentation for [Native.Builder](https://nativelyai.com) (short: **Builder**), built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links before publishing

## Terminology

| Term | Usage |
|------|--------|
| **Native.Builder** | Full product name. Short form: **Builder**. Never use "Natively" for the product. |
| **Builder agent** | The coding agent in the agent roster — always say "Builder agent" to distinguish from the product or the Builder plan |
| **Builder plan** | The $20/mo subscription tier — always say "Builder plan" to distinguish from the product |
| **Software factory** | Core positioning — agents produce software on a production line |
| **Workspace** | The factory floor — team, billing, projects, and members |
| **Project** | One product run through the factory |
| **Agent** | A specialist worker (Product Architect, Builder agent, Task Planner, Feedback) |
| **Credits** | Fuel for agent work — pay for output, not headcount |
| **Publish** | Ship factory output to a live URL on `*.nativelyai.app` |

## Brand assets

Replace logos by dropping files into `/logo/`:

| File | Used for |
|------|----------|
| `logo/light.png` | Navbar on light mode (dark wordmark, transparent BG) |
| `logo/dark.png` | Navbar on dark mode (light wordmark, transparent BG) |
| `logo/icon.png` | Hero card + favicon |

See `logo/README.md` for export specs. **PNG is supported** — replace files in `/logo/` and push; no Mintlify dashboard upload needed.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Link to the live app at `https://nativelyai.com` when referencing in-product actions
- First mention on a page: **Native.Builder**. Subsequent mentions in the same section: **Builder**

## Content boundaries

- Document user-facing product behavior only
- Do not document internal admin tooling, infra, or unreleased features
- Skip troubleshooting pages for now — route users to **Support** instead
- Keep plan details aligned with the in-app pricing page

## Editing workflow

1. Edit the relevant `.mdx` file
2. Run `mint dev` locally to preview
3. Open a PR — Mintlify deploys a preview URL automatically when connected to GitHub
