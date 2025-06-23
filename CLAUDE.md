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

## Issue Management and PR Workflow

This project follows a structured workflow for handling issues and pull requests using GitHub CLI:

### Issue Creation and PR Workflow

1. **Create Issue** (in Japanese):
   ```bash
   gh issue create --title "日本語タイトル" --body "詳細内容"
   ```

2. **Create Branch** (in English, including issue number):
   ```bash
   git checkout -b feature/issue-{number}-brief-description
   # Example: feature/issue-3-add-authentication
   ```

3. **Create Empty Commit and Push**:
   ```bash
   git commit --allow-empty -m "Empty commit for issue #{number}"
   git push -u origin feature/issue-{number}-brief-description
   ```

4. **Create Pull Request** (in Japanese):
   ```bash
   gh pr create --title "日本語PRタイトル" --body "PR description with issue reference"
   ```

5. **Development Process**:
   - Make incremental changes and commit frequently
   - Push changes regularly to keep PR updated
   - Add PR comments to document progress and decisions
   - Use gitmoji and Japanese commit messages
   
   ```bash
   # Make changes, then:
   git add .
   git commit -m "✨ 新機能を追加"
   # or
   git commit -m "🐛 バグを修正"
   # or 
   git commit -m "📝 ドキュメントを更新"
   git push
   
   # Update PR with progress:
   gh pr comment {pr-number} --body "## 進捗更新\n- 実装した機能\n- 次のステップ"
   ```

6. **Update Progress via PR Comments**:
   ```bash
   gh pr comment {pr-number} --body "Progress update message"
   ```

### Workflow Benefits

- **Traceability**: Issue numbers in branch names provide clear connection
- **Early Visibility**: Empty commits and immediate PRs make work visible
- **Continuous Updates**: Regular PR comments keep stakeholders informed
- **Japanese-first**: Issues and PRs use Japanese for better local context, with English branch names for Git convention