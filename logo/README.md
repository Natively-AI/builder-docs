# Logo assets

Mintlify reads these paths from `docs.json`:

| File | When it's used |
|------|----------------|
| **`light.png`** | Navbar in **light mode** — use a **dark** wordmark on transparent background |
| **`dark.png`** | Navbar in **dark mode** — use a **light/white** wordmark on transparent background |
| **`icon.png`** | Hero card mark on the docs home page (optional) |

## Recommended specs

- **Format:** PNG with transparent background
- **Navbar wordmark:** ~160–200px wide, ~32px tall (horizontal lockup with icon + "Native.Builder")
- **Icon only:** 256×256 or 512×512 square

## How to update

1. Export your official assets from Figma/brand kit
2. Replace the files in this folder (same filenames)
3. Commit and push to `main` — Mintlify redeploys automatically

No upload in the Mintlify dashboard is required; the repo **is** the source of truth.

## Current placeholders

The checked-in PNGs are interim icons from the app repo. Replace `light.png` and `dark.png` with your full **Native.Builder** wordmark when ready.
