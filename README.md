# MCP Server Learning

MCP（Model Context Protocol）サーバーの開発を学習するためのTypeScriptプロジェクトです。

## 概要

このプロジェクトは、MCP（Model Context Protocol）の概念を理解し、実際にサーバーを開発するためのハンズオン学習環境を提供します。TypeScriptを使用してMCP（Model Context Protocol）サーバーの基本的な実装を学びます。

## 技術スタック

- **TypeScript**: 型安全性を提供するJavaScriptのスーパーセット
- **Node.js**: JavaScript実行環境
- **CommonJS**: モジュールシステム
- **Strict Mode**: TypeScriptの厳格な型チェックを有効化

## 環境構築

### 前提条件

- Node.js (v14以上推奨)
- pnpm (推奨)

### セットアップ

1. リポジトリをクローン
```bash
git clone https://github.com/ao-39/mcp-server-learning.git
cd mcp-server-learning
```

2. 依存関係をインストール
```bash
pnpm install
```

## 開発コマンド

### TypeScriptコードの実行
```bash
npx ts-node src/index.ts
```

### TypeScriptのコンパイル
```bash
npx tsc
```

### 型チェック
```bash
npx tsc --noEmit
```

### テスト実行
```bash
pnpm test
```
*注: 現在テストは設定されていません*

## プロジェクト構造

```
mcp-server-learning/
├── src/
│   └── index.ts          # メインエントリーポイント
├── node_modules/         # 依存関係
├── package.json          # プロジェクト設定
├── tsconfig.json         # TypeScript設定
├── CLAUDE.md            # Claude Code用の開発支援ドキュメント
└── README.md            # このファイル
```

## 設定詳細

### TypeScript設定
- **ターゲット**: ES2016
- **モジュール**: CommonJS
- **厳格モード**: 全ての型チェックオプションが有効
- **ESモジュール相互運用**: 有効

## 学習目標

1. MCP（Model Context Protocol）の基本概念の理解
2. TypeScriptでのサーバー実装
3. 型安全なコード開発
4. Node.js環境でのMCPサーバー運用

## 貢献

このプロジェクトは学習目的で作成されています。改善提案やバグ報告は、GitHubのIssuesでお知らせください。

