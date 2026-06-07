# Repository Guidelines

## Project Structure & Module Organization
This repository is currently a minimal starting point. `readme.md` is the only project document at the root, and no source, test, or asset directories are present yet. Keep root-level files limited to documentation and project configuration. When implementation begins, prefer conventional top-level folders such as `src/` for application code, `tests/` for automated tests, and `assets/` for static files. Group modules by feature when the codebase grows.

## Build, Test, and Development Commands
No package manager, build system, or test runner is configured yet. Before adding code, document the chosen workflow in `readme.md` and keep this section updated. Expected future examples:

- `npm install`: install JavaScript dependencies when a `package.json` exists.
- `npm test`: run the project test suite.
- `npm run build`: produce production artifacts.
- `make test` or `make build`: use only if a `Makefile` is introduced.

## Coding Style & Naming Conventions
Follow the formatter and linter configured for the language added to the repository. Until tooling exists, keep indentation consistent within each file, use clear descriptive names, and avoid mixing naming styles in the same module. Prefer lowercase, hyphenated filenames for documentation, such as `api-notes.md`. Use language conventions for source files, for example `PascalCase` for React components or `snake_case` for Python modules.

## Testing Guidelines
No tests are configured yet. Add tests alongside the first implementation work, preferably under `tests/` or in language-specific colocated test files. Use predictable names such as `*.test.js`, `*.spec.ts`, or `test_*.py` depending on the stack. Every bug fix should include a regression test when practical. Document any required coverage target once a test framework is selected.

## Commit & Pull Request Guidelines
The current Git history contains only one commit, `init`, so no detailed commit convention has been established. Use short, imperative commit messages, for example `Add contributor guide` or `Implement user settings`. Pull requests should include a concise summary, testing performed, linked issues if applicable, and screenshots for visible UI changes.

## Agent-Specific Instructions
Keep repository changes focused and avoid unrelated formatting churn. If new tooling, source directories, or test commands are added, update this guide in the same change.
