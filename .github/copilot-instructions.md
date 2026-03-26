# GitHub Copilot Instructions

This file provides guidance to GitHub Copilot when working with this TypeScript project.

## Project Overview

**ai-typescript-starter** is an AI-native TypeScript starter template designed for the AI-assisted development era.

## Code Style Guidelines

- Use 2-space indentation
- Use single quotes for strings
- Always use semicolons
- Maximum line width: 100 characters
- Avoid `any` type - use specific types or generics
- Use `const` for variables that don't change, `let` only when necessary

## Naming Conventions

- **Files**: Use kebab-case for filenames (e.g., `my-module.ts`)
- **Classes**: Use PascalCase (e.g., `MyClass`)
- **Functions/Variables**: Use camelCase (e.g., `myFunction`)
- **Constants**: Use SCREAMING_SNAKE_CASE for true constants (e.g., `MAX_RETRY_COUNT`)
- **Types/Interfaces**: Use PascalCase (e.g., `UserConfig`)

## TypeScript Best Practices

- Enable strict mode
- Define explicit return types for public functions
- Use interfaces for object shapes
- Use type aliases for unions, intersections, and utility types
- Prefer `unknown` over `any` for truly unknown types
- Use optional chaining (`?.`) and nullish coalescing (`??`)

## Testing Guidelines

- Write tests in `__tests__` directories or adjacent `.test.ts` files
- Use Vitest for testing
- Aim for 80% test coverage
- Test edge cases and error conditions
- Use descriptive test names

## Available Scripts

```bash
pnpm run build      # Build the project
pnpm run dev        # Development mode with watch
pnpm run test       # Run tests
pnpm run lint       # Lint code
pnpm run typecheck  # Type check
pnpm run check      # Full check (typecheck + lint)
```

## Commit Message Format

Follow Conventional Commits:

- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation only
- `style:` - Code style changes (formatting, etc.)
- `refactor:` - Code refactoring
- `perf:` - Performance improvement
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks

## Architecture

```
src/
├── index.ts          # Main entry point
├── [module].ts       # Feature modules
└── __tests__/        # Test files
    └── [module].test.ts
```