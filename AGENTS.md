# native.builder documentation

## About this project

- Product documentation for [native.builder](https://nativelyai.com) (short: **Builder**), built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links before publishing

## Terminology

| Term | Usage |
|------|--------|
| **native.builder** | Full product name — always lowercase (`native.builder`), optionally with the `brand-name` class for small-caps styling. Short form: **Builder**. Never use "Natively" for the product. |
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
- First mention on a page: **native.builder** (lowercase). Subsequent mentions in the same section: **Builder**

## Content boundaries

- Document user-facing product behavior only
- Do not document internal admin tooling, infra, or unreleased features
- Skip troubleshooting pages for now — route users to **Support** instead
- Keep plan details aligned with the in-app pricing page

## Public changelog

`changelog.mdx` is the public product changelog. Keep the existing structure:

```mdx
## vX.Y.Z — Month YYYY

### New
- **Feature name** — Short user-facing benefit

### Improved
- **Area** — What got better for the user

### Fixed
- **Area** — What works again / correctly now
```

Rules for changelog entries (humans and automations):

- Only ship changes that affect how customers build, collaborate, or ship in **native.builder**
- Prefer source text from `Natively-AI/conductor-2.0` files matching `changelog/v*-user.md` — those are the approved public summaries
- Ignore engineering-only notes in `changelog/vX.Y.Z.md` (no `-user` suffix)
- Match terminology in this file; never call the product "Natively"
- Map section names: What's new → New, Improvements → Improved, Fixes → Fixed, Removed → Removed
- Insert newer versions above older ones, directly under the intro paragraph
- Do not change older published entries unless correcting a factual error
- Open a PR for review; do not push straight to `main` unless explicitly configured to automerge

## Editing workflow

1. Edit the relevant `.mdx` file
2. Run `mint dev` locally to preview
3. Open a PR — Mintlify deploys a preview URL automatically when connected to GitHub
