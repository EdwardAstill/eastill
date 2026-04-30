# GitHub Project Catalog

Checked on 2026-04-30 from GitHub metadata and repository READMEs visible to
the `EdwardAstill` account. Updated after deleting `stcalc_cli`, `notey`,
`note_app`, `storm`, `coaches`, `rustycube`, `shotty`, `dock-ui`, and `SQL`.

## Inventory summary

| Metric | Count |
|---|---:|
| Total repositories checked | 47 |
| Public repositories | 26 |
| Private repositories | 21 |
| Repositories with a README | 41 |
| Repositories missing a README | 6 |
| Forks | 0 |

## Documentation backlog

| Priority | Repositories | Work needed |
|---|---|---|
| Missing public README | `monopoly-deal`, `swapbeat` | Add a short README explaining the project, current status, how to run it, and whether it is active or archived. |
| Missing private README | `UNI-26-1`, `uni-25-2`, `uni-25-1`, `nostalgia` | Add at least a private maintenance README so future agents can identify purpose and state. |
| Weak or placeholder README | `plan`, `pyseasfem`, `AI` | Replace scaffolding, bare links, or empty README bodies with a real project summary. |
| Encoding-damaged README | `config`, `routines` | Re-save as UTF-8 and rewrite the opening section. |
| Public profile cleanup | `convert2`, `m8s`, `terminal-art`, `connecty`, `beamy`, `unity` | Add or improve GitHub descriptions where blank, so the profile can be generated from metadata more reliably. |

## Agent systems and automation

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`warden`](https://github.com/EdwardAstill/warden) | Private | Agent capability layer: skills, subagents, hooks, modes, and CLI tooling mirrored across Claude Code, Codex, Gemini, and other harnesses. | Strong README. | Keep private unless there is a deliberate public release plan. |
| [`gwt`](https://github.com/EdwardAstill/gwt) | Public | Git worktree helper that creates a sibling worktree, allocates a free TCP port, emits a `WORKTREE CONTEXT` block, and can launch a command inside the worktree. | Strong README. | Keep in the public profile as a clear, practical dev tool. |
| [`termread`](https://github.com/EdwardAstill/termread) | Public | Captures terminal scrollback from tmux, screen, stdin, or live commands so an agent can inspect shell output it did not produce. | Strong README. | Keep paired with other agent utilities in the profile. |
| [`foxpilot`](https://github.com/EdwardAstill/foxpilot) | Private | Firefox automation CLI and MCP server for AI agents, with dedicated automation, attach-to-Zen, and headless modes. | Strong README. | Decide later whether any public subset is safe to expose. |
| [`webscraper`](https://github.com/EdwardAstill/webscraper) | Public | Pure-HTTP scraping CLI for inspecting URLs, scaffolding scraper scripts, fetching pages with browser-like headers, and exporting data. | Strong README. | Keep public and grouped with automation tools. |
| [`yt-tool`](https://github.com/EdwardAstill/yt-tool) | Public | YouTube CLI/TUI for transcripts, audio/video download, summaries, channel and playlist listing, and search. | Strong README. | Keep public; update repo description to match current larger scope. |
| [`arch-viewer`](https://github.com/EdwardAstill/arch-viewer) | Public | CLI plus React viewer that scans Python and TypeScript projects into a navigable architecture graph. | Strong README. | Keep public; add screenshots later if useful. |
| [`coach-plugin`](https://github.com/EdwardAstill/coach-plugin) | Public | Claude Code plugin that scaffolds domain-specific AI coaches from a `/create-coach` command. | Strong README. | Keep public. |
| [`secrets`](https://github.com/EdwardAstill/secrets) | Private | Small CLI for managing API keys and env vars in a chmod-600 file at `~/.secrets`. | Useful README. | Keep private or rename before any public release to avoid confusion with secret material. |
| [`pl-AI-giarism`](https://github.com/EdwardAstill/pl-AI-giarism) | Private | Web app and CLI-friendly backend for running text through multiple AI and plagiarism assessors. | Useful README. | Keep private; improve name/status note if it stays active. |

## Knowledge, documents, and conversion

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`readrun`](https://github.com/EdwardAstill/readrun) | Public | Turns folders of Markdown into interactive websites with executable Python code blocks. | Strong README. | Keep public and feature prominently. |
| [`markstore`](https://github.com/EdwardAstill/markstore) | Public | Local markdown store with SQLite, full-text search, semantic vector search, and knowledge graph querying. | Strong README. | Keep public and link from knowledge tooling. |
| [`wiki-pro`](https://github.com/EdwardAstill/wiki-pro) | Public | LLM-first CLI for searching, reading sections, listing tags, validating, and traversing markdown wikis. | Strong README. | Keep public and group near `markstore`. |
| [`knowledge`](https://github.com/EdwardAstill/knowledge) | Private | Structured markdown knowledge base covering computing, finance, math, chemistry, economics, engineering, health, and related source notes. | Useful README. | Keep private; do not expose note contents in the profile. |
| [`notes`](https://github.com/EdwardAstill/notes) | Private | Older or alternate structured markdown knowledge base. | Minimal README. | Decide whether this is superseded by `knowledge`; archive or add a status note. |
| [`convert2`](https://github.com/EdwardAstill/convert2) | Public | PDF-first converter, exposed as `cnv`, for producing local AI-friendly Markdown from PDFs and directories of PDFs. | Strong README; GitHub description blank. | Add GitHub description and keep public. |
| [`mdtyp`](https://github.com/EdwardAstill/mdtyp) | Public | Markdown-to-Typst converter with CLI and interactive browser modes, mapping markdown constructs into Typst output. | Strong README. | Keep public; link from document tooling section. |
| [`courses`](https://github.com/EdwardAstill/courses) | Private | Quiz-first course project built with `readrun`, including course content, docs, examples, preview material, and hosting plan. | Useful README. | Keep private unless course content is ready for public release. |
| [`eastill`](https://github.com/EdwardAstill/eastill) | Public | GitHub profile repo and index of projects. | Improved by this change. | Maintain from this catalog. |
| [`pyagrams`](https://github.com/EdwardAstill/pyagrams) | Private | Python diagramming library for creating SVG diagrams with a clean code API and styling system. | Strong README. | Consider public release if it becomes generally useful. |
| [`annas-cli`](https://github.com/EdwardAstill/annas-cli) | Private | CLI for searching, downloading, and batch handling files from Anna's Archive. | Useful README. | Keep private. |

## Engineering, analysis, and research

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`connecty`](https://github.com/EdwardAstill/connecty) | Public | Weld connection analysis from DXF geometry, applied forces/moments, elastic or ICR analysis, AISC 360-22 checks, and SVG plotting. | Useful README. | Add a GitHub description and keep public. |
| [`beamy`](https://github.com/EdwardAstill/beamy) | Public | Beam analysis library covering materials, sections, supports, loads, solving, results, and visualisation. | Useful README. | Add a GitHub description and tighten the README opening. |
| [`sectiony`](https://github.com/EdwardAstill/sectiony) | Public | Section properties and stress analysis for structural cross-sections, including standard shapes such as CHS, RHS, I, channel, SHS, angle, and T sections. | Useful README. | Keep public; consider example gallery. |
| [`unity`](https://github.com/EdwardAstill/unity) | Public | Unit conversion and quantity arithmetic system for engineering scripts, including scalar and array quantities. | Useful README. | Add a clearer GitHub description. |
| [`FanMin`](https://github.com/EdwardAstill/FanMin) | Private | University thesis research project around Point Alpha methodology for engineering fatigue-data scatter and guideline bounds. | Strong README. | Keep private while research is not ready for public presentation. |
| [`pyseasfem`](https://github.com/EdwardAstill/pyseasfem) | Private | Early finite-element-method / solid-mechanics solver notes and module outline. | Weak README. | Replace generated outline with project purpose, current state, and next steps. |

## UI, TUI, media, and creative tools

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`reacterm`](https://github.com/EdwardAstill/reacterm) | Public | React-based compositor-driven terminal UI framework; README presents the project as Storm. | Strong README. | Clarify naming between `reacterm` repo and Storm branding. |
| [`ui`](https://github.com/EdwardAstill/ui) | Public | Living style reference and UI component sandbox for future applications. | Useful README. | Keep public; link from profile as design language. |
| [`terminal-art`](https://github.com/EdwardAstill/terminal-art) | Public | React/TypeScript editor for ANSI and ASCII art on a shared grid canvas. | Strong README; GitHub description blank. | Add GitHub description and screenshots later. |
| [`pdfkit`](https://github.com/EdwardAstill/pdfkit) | Public | Fully client-side browser PDF editor and annotation tool. | Strong README. | Keep public and add demo/screenshot if available. |
| [`m8s`](https://github.com/EdwardAstill/m8s) | Public | Browser-based DAW with text-editable project format and MCP support for AI-assisted composition. | Strong README; GitHub description blank. | Add GitHub description. |
| [`speaknote-py`](https://github.com/EdwardAstill/speaknote-py) | Public | Offline push-to-talk speech-to-text TUI using Vosk, with save/copy workflow and no cloud dependency. | Strong README. | Keep public and group with local-first tools. |
| [`dash`](https://github.com/EdwardAstill/dash) | Private | Personal operations dashboard with web UI and terminal UI served by a single Bun-backed local binary. | Strong README. | Keep private; summarize publicly only at a high level. |
| [`monopoly-deal`](https://github.com/EdwardAstill/monopoly-deal) | Public | HTML game implementation experiment for Monopoly Deal. | Missing README. | Add README or archive. |
| [`swapbeat`](https://github.com/EdwardAstill/swapbeat) | Public | TypeScript experiment, likely music or rhythm related. | Missing README. | Add README before featuring. |
| [`tasky`](https://github.com/EdwardAstill/tasky) | Public | Terminal daily task-management application. | Basic README. | Tighten README structure and add install/run instructions. |
| [`plan`](https://github.com/EdwardAstill/plan) | Private | Planning app or site; README currently points to a deployed URL only. | Weak README. | Add project purpose, stack, and status. |
| [`nostalgia`](https://github.com/EdwardAstill/nostalgia) | Private | HTML experiment. | Missing README. | Add purpose/status or archive. |

## Personal systems, config, and small utilities

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`dotfiles`](https://github.com/EdwardAstill/dotfiles) | Private | Personal Arch/EndeavourOS Hyprland dotfiles, setup scripts, stow packages, theme switching, key bindings, and monitor configuration. | Strong README. | Keep private unless audited for secrets and personal paths. |
| [`config`](https://github.com/EdwardAstill/config) | Private | Lua configuration repo. | Encoding-damaged README. | Repair encoding and explain relationship to `dotfiles`. |
| [`routines`](https://github.com/EdwardAstill/routines) | Private | Personal routines repository. | Encoding-damaged README. | Keep private; repair README if it will remain active. |
| [`tmee`](https://github.com/EdwardAstill/tmee) | Public | Small CLI for printing a folder tree. | Minimal README. | Keep public; add examples and flags. |
| [`AI`](https://github.com/EdwardAstill/AI) | Private | Python AI learning or utility repository. | README present but not informative. | Add purpose/status or archive. |

## University and archive material

| Project | Visibility | What it is | README state | Next action |
|---|---|---|---|---|
| [`UNI-26-1`](https://github.com/EdwardAstill/UNI-26-1) | Private | University unit work for 2026 semester 1. | Missing README. | Add private README with units, constraints, and archive status. |
| [`uni-25-2`](https://github.com/EdwardAstill/uni-25-2) | Private | University unit work for 2025 semester 2. | Missing README. | Add private README or archive. |
| [`uni-25-1`](https://github.com/EdwardAstill/uni-25-1) | Private | University unit work for 2025 semester 1. | Missing README. | Add private README or archive. |

## Profile-ready public set

These public repos have enough description to be shown in the GitHub profile
now:

`gwt`, `yt-tool`, `webscraper`, `termread`, `coach-plugin`,
`arch-viewer`, `markstore`, `readrun`, `wiki-pro`, `convert2`, `mdtyp`,
`connecty`, `beamy`, `sectiony`, `unity`, `reacterm`, `ui`, `terminal-art`,
`pdfkit`, `m8s`, `speaknote-py`, `tmee`, `tasky`.

These public repos should not be highlighted until a README exists or their
status is made clear:

`monopoly-deal`, `swapbeat`.
