# Edward Astill

Structural engineering student and builder of local-first tools for engineering,
AI-assisted development, documents, knowledge systems, and terminal/web
interfaces.

I like small tools that do real work: CLIs that turn messy inputs into useful
files, engineering calculators with inspectable assumptions, agent workflows
that can be routed and audited, and UI experiments that make the terminal feel
less cramped.

## Current focus

| Area | What I am building |
|---|---|
| Agent systems | Skills, hooks, browser control, repo-aware planning, and small utilities that help coding agents operate with better context. |
| Engineering tools | Structural analysis, unit handling, connection checks, PDF/document workflows, and research tooling for fatigue data. |
| Knowledge systems | Markdown stores, wiki navigation, executable docs, conversion pipelines, and course/learning infrastructure. |
| Interfaces | React/TypeScript UI, terminal UI, ANSI art tooling, browser tools, and local-first dashboards. |

## Project map

This repo is the public profile surface. The fuller maintenance view lives in
[`docs/projects`](docs/projects/README.md):

- 47 GitHub repositories checked on 2026-04-30 after repository cleanup.
- 26 public repositories and 21 private repositories were visible to the GitHub token.
- 41 repositories had a README; 6 were missing one.
- Private repos are visibility-labelled in the catalog so they are not confused with public portfolio material.

## Public projects

### Agent tools and automation

| Repo | What it is |
|---|---|
| [`gwt`](https://github.com/EdwardAstill/gwt) | Git worktree helper that creates branch worktrees, allocates a free dev port, and prints a machine-readable context block. |
| [`yt-tool`](https://github.com/EdwardAstill/yt-tool) | YouTube CLI and TUI for transcripts, audio/video downloads, summaries, playlist/channel listing, and search. |
| [`webscraper`](https://github.com/EdwardAstill/webscraper) | Pure-HTTP scraping CLI for inspecting pages, fetching URLs, and scaffolding scraper scripts. |
| [`termread`](https://github.com/EdwardAstill/termread) | Captures terminal scrollback from tmux, screen, stdin, or live commands so agents can inspect output they did not run. |
| [`coach-plugin`](https://github.com/EdwardAstill/coach-plugin) | Claude Code plugin that scaffolds domain-specific AI coaches from a single command. |
| [`arch-viewer`](https://github.com/EdwardAstill/arch-viewer) | CLI plus React viewer that scans Python/TypeScript projects and renders an architecture graph. |

### Knowledge, docs, and conversion

| Repo | What it is |
|---|---|
| [`markstore`](https://github.com/EdwardAstill/markstore) | Local markdown database with full-text search, vector search, and knowledge-graph queries. |
| [`readrun`](https://github.com/EdwardAstill/readrun) | Turns Markdown folders into interactive websites with executable Python code blocks. |
| [`wiki-pro`](https://github.com/EdwardAstill/wiki-pro) | LLM-first CLI for searching, reading, and traversing structured markdown wikis. |
| [`convert2`](https://github.com/EdwardAstill/convert2) | PDF-first converter that turns PDFs into local, AI-friendly Markdown. |
| [`mdtyp`](https://github.com/EdwardAstill/mdtyp) | Markdown-to-Typst converter with a command-line path and interactive file browser. |
| [`eastill`](https://github.com/EdwardAstill/eastill) | This profile repo and project index. |

### Engineering and analysis

| Repo | What it is |
|---|---|
| [`connecty`](https://github.com/EdwardAstill/connecty) | Weld connection analysis from DXF geometry, applied loads, elastic/ICR analysis, AISC checks, and SVG plots. |
| [`beamy`](https://github.com/EdwardAstill/beamy) | Beam analysis library for materials, sections, supports, loads, solving, results, and visualisation. |
| [`sectiony`](https://github.com/EdwardAstill/sectiony) | Section-property and stress-analysis library for common structural cross-sections. |
| [`unity`](https://github.com/EdwardAstill/unity) | Unit conversion and quantity arithmetic system for engineering scripts. |

### UI, media, and creative systems

| Repo | What it is |
|---|---|
| [`reacterm`](https://github.com/EdwardAstill/reacterm) | React-based compositor-driven terminal UI framework, presented as Storm in its README. |
| [`ui`](https://github.com/EdwardAstill/ui) | Living style reference and UI component sandbox for future apps. |
| [`terminal-art`](https://github.com/EdwardAstill/terminal-art) | React/TypeScript editor for ANSI and ASCII art on a shared grid canvas. |
| [`pdfkit`](https://github.com/EdwardAstill/pdfkit) | Browser-based PDF editor and annotation tool that runs fully client-side. |
| [`m8s`](https://github.com/EdwardAstill/m8s) | Browser-based DAW with text-editable project files and MCP support for AI-assisted composition. |
| [`speaknote-py`](https://github.com/EdwardAstill/speaknote-py) | Offline push-to-talk speech-to-text TUI built on Vosk. |

### Smaller tools and experiments

| Repo | What it is |
|---|---|
| [`tmee`](https://github.com/EdwardAstill/tmee) | Small CLI for printing a folder tree. |
| [`tasky`](https://github.com/EdwardAstill/tasky) | Terminal-based daily task manager. |
| [`monopoly-deal`](https://github.com/EdwardAstill/monopoly-deal) | Browser game experiment; README is still missing. |
| [`swapbeat`](https://github.com/EdwardAstill/swapbeat) | TypeScript experiment; README is still missing. |

## Documentation status

The project catalog now tracks what each repo is, whether it is public or
private, and what documentation work is needed next. The highest-impact cleanup
items are:

- Add READMEs for public repos that are missing them: `monopoly-deal` and `swapbeat`.
- Clean up older private READMEs with encoding damage or placeholder content.
- Keep this profile README focused on public, portfolio-safe projects.
- Use [`docs/projects/catalog.md`](docs/projects/catalog.md) as the working
  source for future project descriptions.

## Contact

[edwardast.ll@gmail.com](mailto:edwardast.ll@gmail.com)
