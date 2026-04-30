# Plan: Profile And Project Catalog Overhaul

**Created:** 2026-04-30T07:48Z
**Status:** approved
**Shape:** research-plan-execute-review
**Human checkpoints:** 1
**Refinement passes:** 1

## Goal

Turn `EdwardAstill/eastill` from a short repository list into a stronger public
portfolio hub backed by a maintainable project catalog sourced from the actual
GitHub READMEs.

## Research findings

- Current repo is `EdwardAstill/eastill`, the GitHub profile repository.
- The local repo had only `README.md` before this work.
- GitHub inventory found 56 repositories visible to the authenticated account.
- Visibility split: 28 public, 28 private.
- README coverage: 48 present, 8 missing.
- One visible repo is a fork: `storm`.
- Missing READMEs: `UNI-26-1`, `dock-ui`, `monopoly-deal`, `swapbeat`,
  `uni-25-2`, `rustycube`, `uni-25-1`, `nostalgia`.

## Sub-tasks

### Sub-task 1 - Inventory GitHub repositories and READMEs

**Block:** research
**Skill:** github
**Depends on:** none

**Instruction:**

Use `gh repo list EdwardAstill --limit 200` and `gh api
repos/<owner>/<repo>/readme` to enumerate every visible GitHub repository,
capture visibility, language, pushed date, description, README presence,
README title, opening paragraph, and headings.

**Inputs (pre-staged):**
- command: `gh repo list EdwardAstill --limit 200`
- command: `gh api repos/<owner>/<repo>/readme`

**Acceptance:**
- `jq 'length' /tmp/eastill-repos.json` prints `56`.
- `rg '^- README: missing' /tmp/eastill-readme-inventory-fixed.md | wc -l` prints `8`.

### Sub-task 2 - Create project explainer folder

**Block:** execute
**Skill:** docs-writing
**Depends on:** Sub-task 1

**Instruction:**

Create `docs/projects/README.md` and `docs/projects/catalog.md`. The folder
must explain that it is the maintenance view behind the public profile README.
The catalog must include all 56 repositories with visibility, purpose, README
state, and next documentation action.

**Inputs (pre-staged):**
- file: `/tmp/eastill-repos.json`
- file: `/tmp/eastill-readme-inventory-fixed.md`

**Acceptance:**
- `test -f docs/projects/README.md`
- `test -f docs/projects/catalog.md`
- `rg -F '| Total repositories checked | 56 |' docs/projects/catalog.md`
- `rg 'monopoly-deal.*Missing README' docs/projects/catalog.md`

### Sub-task 3 - Rewrite public profile README

**Block:** execute
**Skill:** docs-writing
**Depends on:** Sub-task 2

**Instruction:**

Rewrite `README.md` as a stronger GitHub profile surface. It should open with a
clear positioning statement, list current focus areas, group public projects by
theme, link to `docs/projects`, and avoid treating private repos as public
portfolio links.

**Inputs (pre-staged):**
- file: `README.md`
- file: `docs/projects/catalog.md`

**Acceptance:**
- `rg 'Current focus' README.md`
- `rg 'docs/projects/catalog.md' README.md`
- `rg '\\[warden\\]' README.md` exits non-zero, because private repos should not be promoted from the public profile.

### Sub-task 4 - Track README cleanup backlog

**Block:** execute
**Skill:** docs-writing
**Depends on:** Sub-task 2

**Instruction:**

Add a documentation backlog to the catalog that names missing public READMEs,
missing private READMEs, weak placeholder READMEs, encoding-damaged READMEs,
and metadata cleanup opportunities.

**Inputs (pre-staged):**
- file: `/tmp/eastill-readme-inventory-fixed.md`
- file: `docs/projects/catalog.md`

**Acceptance:**
- `rg 'Missing public README' docs/projects/catalog.md`
- `rg 'Encoding-damaged README' docs/projects/catalog.md`
- `rg 'Weak or placeholder README' docs/projects/catalog.md`

### Sub-task 5 - Privacy and publication checkpoint

**Block:** human
**Skill:** ask
**Depends on:** Sub-task 2, Sub-task 3, Sub-task 4

**Instruction:**

Before pushing this public profile repository, review whether the private
repository names and summaries in `docs/projects/catalog.md` are acceptable to
publish. If not, split the catalog into a public tracked file and a private
untracked maintenance file.

**Inputs (pre-staged):**
- file: `docs/projects/catalog.md`

**Acceptance:**
- Human confirms private repo names are acceptable in this repo, or catalog is split before publication.

### Sub-task 6 - Verify documentation structure

**Block:** review
**Skill:** verification-before-completion
**Depends on:** Sub-task 2, Sub-task 3, Sub-task 4

**Instruction:**

Run lightweight verification for markdown structure, internal links, and diff
cleanliness. Confirm that every public repo in the current profile README exists
in the GitHub inventory and every new docs file is linked from the root README
or `docs/projects/README.md`.

**Inputs (pre-staged):**
- file: `README.md`
- file: `docs/projects/README.md`
- file: `docs/projects/catalog.md`

**Acceptance:**
- `git diff --check`
- `rg 'docs/projects/README.md|docs/projects/catalog.md' README.md`
- `rg '^## Files' docs/projects/README.md`

### Sub-task 7 - Next wave: improve source repository READMEs

**Block:** execute
**Skill:** docs-writing
**Depends on:** Sub-task 5

**Instruction:**

In a later session, visit the source repositories named in the backlog and add
or repair their READMEs. Start with public repos missing READMEs
(`monopoly-deal`, `swapbeat`), then weak public docs, then private repo cleanup.

**Inputs (pre-staged):**
- file: `docs/projects/catalog.md`

**Acceptance:**
- Each source repo has at least: what it is, install/run instructions if applicable, current status, and license/status note.
- Profile README no longer needs to compensate for missing project descriptions.
