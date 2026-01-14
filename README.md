# mcp_work

## 概要
このリポジトリはMCP（Model Context Protocol）統合のためのワークスペースです。
概要変更しました。

## プロジェクト構成

### ディレクトリ構造
- `.git/` - Gitリポジトリ
- `.github/` - GitHub設定（Copilot Instructionsを含む）
- `.vscode/` - VS Code設定（MCP server設定を含む）
- `README.md` - プロジェクトドキュメント

### MCP Server設定
`.vscode/mcp.json`でリモートMCPサーバーへの接続が構成されています：
- URL: https://api.githubcopilot.com/mcp/
- Type: http

## 特徴
- 設定駆動型のプロジェクト構成
- リモートMCPサーバーとの統合
- VS Code環境での開発をサポート

## Docker使用例
GitHub MCP serverをローカルで実行する場合：
```sh
docker run --rm -i -e GITHUB_PERSONAL_ACCESS_TOKEN ghcr.io/github/github-mcp-server
```

*注: 有効な`GITHUB_PERSONAL_ACCESS_TOKEN`を環境変数に設定する必要があります。*

## 拡張方法
- MCPワークフローに必要なソースコード、スクリプト、ドキュメントを追加
- `.vscode/mcp.json`を更新して追加のサーバーや入力を設定
