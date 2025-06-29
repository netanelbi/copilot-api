# OpenCode.md

## Build, Lint & Test Commands
- Install dependencies: `bun install`
- Build: `bun run build`
- Dev server (watch): `bun run dev`
- Production start: `bun run start`
- Lint: `bun run lint`
- Test (all): `bun test`
- Test (single file): `bun test src/<file>.spec.ts`

## Code Style Guidelines
- **Imports**: Use ES6 modules; sort imports logically (external libraries first, then relative paths).
- **Formatting**: Follow Prettier conventions (`prettier-plugin-packagejson` is active).
- **Types**: Prefer explicit types in TypeScript; avoid `any` unless strictly necessary.
- **Naming**: Use camelCase for variables/functions, PascalCase for classes/types, SCREAMING_SNAKE_CASE for constants.
- **Error Handling**: Centralize error management using utils from `src/lib/error.ts`.
- **Language Features**: Modern ES6+ syntax preferred.
- **Contextual Guidelines**: Match existing patterns seen across `/src/lib` and `/src/services`.

## Other Notes
- Follow TypeScript/Bun/ESLint conventions (`eslint.config.js` applies).
- Tokens and cache are handled automatically; authentication is CLI-rooted.