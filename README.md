# genie-public-assets

Public assets used as defaults for Genie / Claude Code Academy public content — Notion page icons and covers, slide-deck logos, screenshots referenced from skills, and similar.

This repo is **public** because tools like Notion fetch raw image URLs anonymously and silently fail on private repos. Do not put anything sensitive here.

## Layout

```
assets/
  icon.png      — default Notion page icon (square, 280x280 or 512x512, transparent PNG)
  banner.png    — default Notion page cover (1500x600, 5:2, content centered vertically)
```

## Raw URLs

Use the `raw.githubusercontent.com` form so the URL serves the image directly:

```
https://raw.githubusercontent.com/Claude-Code-Academy/genie-public-assets/main/assets/icon.png
https://raw.githubusercontent.com/Claude-Code-Academy/genie-public-assets/main/assets/banner.png
```

## Updating an image

Push a new version of the same filename to `main`. Existing references pick up the new image the next time the consuming service refreshes its cache (Notion typically within a minute).

## Used by

- `genie-notion-tools` plugin in [`amirthan/genie-internal-plugins`](https://github.com/amirthan/genie-internal-plugins) — both `notion-page-editor` (every Notion page rewrite) and `genie-update-github-guides` (every GitHub-guide page refresh).

## License

CC0 — no rights reserved. Anyone can reuse these images. See `LICENSE`.
