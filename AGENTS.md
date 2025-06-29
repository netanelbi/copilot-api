AGENTS.md

# Agent Coding Guidelines

**Build/Lint/Test Commands**

- Install: `bun install`
- Build: `bun run build`
- Lint: `bun run lint` (auto-fix: `bunx eslint --fix`)
- Dev server: `bun run dev`
- Production: `bun run start`
- Run all tests: _No test script found; add one if needed_
- Run single test: _No test script found; add one if needed_

**Code Style**

- Use TypeScript strict mode; all code must be type-safe.
- Prefer named imports; use `import { foo } from "bar"` style.
- Use ESNext module syntax and features.
- Use `~/` alias for `src/` imports.
- Use concise arrow functions and `const`/`let` (never `var`).
- Function, variable, and file names: camelCase; types/interfaces: PascalCase.
- Handle errors with custom `HTTPError` and `forwardError` (`src/lib/error.ts`).
- No comments unless required; keep code self-explanatory.
- No unused variables/parameters; keep code clean.
- Format with Prettier defaults (2 spaces, single quotes, trailing commas).
- Use `consola` for logging.
- Do not add AGENTS.md, .cursorrules, or copilot-instructions.md unless requested.
