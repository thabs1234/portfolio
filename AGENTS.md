# AGENTS.md

> Agent/AI coding rules for this project. Loaded automatically by tools
> that read project context (Cursor, Claude, Codex, Hermes). Merge with any
> project-specific instructions below.

## Behavioral Guidelines (Karpathy-Inspired)

These bias toward caution over speed — use judgment on trivial tasks.

### 1. Think Before Coding
- State assumptions explicitly; ask when uncertain.
- Never silently pick between multiple interpretations — present them.
- If a simpler approach exists, say so and push back.
- Low-stakes ambiguity: pick a sensible default, state it, proceed.

### 2. Simplicity First
- Minimum code that solves the problem. No speculative features/abstractions.
- Handle errors only at real I/O / system boundaries; skip the impossible.

### 3. Surgical Changes
- Read the code before editing — never edit blind.
- Touch only what the request requires; match existing style.
- Remove only orphans your change created. Mention (don't delete) other dead code.
- After changes: show what changed and how you verified it.

### 4. Goal-Driven Execution
- Turn tasks into verifiable goals (write a failing test, then make it pass).
- State a brief plan with a check per step.
- Verify against real output, not self-reports. After ~3 failed fixes, stop and report the blocker.

## Project-Specific Instructions

- **Type:** Static site — plain HTML/CSS/JS. No framework, no build step, no package manager.
- **Files:** `index.html` (markup), `style.css` (styles), `script.js` (behavior), `README.md`.
- **Conventions:** Vanilla JS (no bundler); keep CSS readable, no preprocessor; match existing class naming.
- **Edit, don't rewrite:** prefer targeted edits to `index.html` / `style.css` / `script.js`.
- **Verify:** open `index.html` in a browser or serve with `python -m http.server` and confirm the change renders/behaves as intended.
- **Not yet a git repo:** `git init` before committing. Deploy target is GitHub Pages (thabs1234.github.io/portfolio).
