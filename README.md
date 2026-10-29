# Prep Hub — AI / GenAI Internship Roadmap

A responsive, single-page checklist based on an AI/GenAI internship skill target. It includes:

- Overall completion percentage and Basic/Core/Pro progress bars
- Seven collapsible learning phases and project milestones
- Search, All / To do / Completed filters, and a next-task shortcut
- Custom tasks
- Automatic progress saving in the current browser (`localStorage`)
- JSON export/import for backups and moving progress between browsers
- No build tools, server, external libraries, or API keys required

## Run locally

Open `index.html` in a browser. For a local web server, run this from the project directory:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a GitHub repository (for example, `prep-hub-roadmap`).
2. Upload `index.html` and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site; use the URL shown on the Pages settings screen.

## Progress and privacy

Your checklist and custom tasks are saved in the browser's local storage for this site's URL. They are not sent to a server, and the site does not have accounts or cloud sync. Export a JSON backup before clearing browser data or moving to another device. Import that backup on the other device to restore progress.

## Updating the roadmap

Built-in tasks live in the `phases` array inside `index.html`. Each task has a stable `id`, `title`, `description`, `tier`, and optional `time`. Keep IDs stable if you change a task title; progress is tracked by ID.
