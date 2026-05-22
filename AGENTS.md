# AGENTS.md

## Cursor Cloud specific instructions

This is a **static HTML/CSS e-commerce site** using Bootstrap 5 (loaded via CDN). There is no build system, no package manager, no backend, and no external dependencies.

### Running the development server

```bash
python3 -m http.server 8000
```

This serves all files from the workspace root at `http://localhost:8000/`. The main entry point is `index.html`.

### Project structure

- `index.html` — Main homepage (and entry point)
- `instructions-agent.md` — Build plan (in French) describing the 5-day integration schedule
- `RECAP.md` — Summary of completed work

### Key notes

- No `npm install`, `pip install`, or other dependency installation is needed.
- No linter or test framework is configured. When HTML/CSS linting is needed, use an external tool like `npx htmlhint index.html` (htmlhint can be run via npx without prior installation).
- Bootstrap 5 is loaded via CDN links in the HTML files — no local installation required.
- The project is built incrementally (one page per day) following `instructions-agent.md`.
