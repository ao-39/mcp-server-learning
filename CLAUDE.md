# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a TypeScript project for learning MCP (Model Context Protocol) server development. The project uses:

- **TypeScript** with CommonJS modules
- **Node.js** runtime
- **Strict type checking** enabled
- **Basic project structure** with source code in `src/`

## Development Commands

**Run TypeScript code:**
```bash
npx ts-node src/index.ts
```

**Compile TypeScript:**
```bash
npx tsc
```

**Type checking:**
```bash
npx tsc --noEmit
```

## Project Structure

- `src/index.ts` - Main entry point (currently just a hello world)
- `tsconfig.json` - TypeScript configuration with strict mode enabled
- `package.json` - Project dependencies and scripts

## Key Configuration

- **TypeScript target:** ES2016
- **Module system:** CommonJS
- **Strict mode:** Enabled for all type checking
- **Source map support:** Available but not currently enabled