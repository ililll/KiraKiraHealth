# KiraKiraHealth

> SaaS アプリケーション（プロダクト概要は [docs/product/vision.md](docs/product/vision.md)、届ける価値の定義は [docs/product/value-definition.md](docs/product/value-definition.md) を参照）

## リポジトリ構成

```
.
├── apps/                  # デプロイ単位のアプリケーション
│   ├── web/               # フロントエンド（Web UI）
│   └── api/               # バックエンド（API サーバー）
├── packages/              # apps 間で共有するライブラリ（型定義・UI部品・ユーティリティ等）
├── infra/                 # IaC（Terraform 等）・環境構成
├── scripts/               # 開発・運用用スクリプト
├── docs/
│   ├── product/           # プロダクトビジョン・ペルソナ・ロードマップ
│   ├── agile/             # DoR / DoD / スプリント運用ルール・テンプレート
│   ├── sprints/           # 各スプリントの計画・レビュー・レトロ記録
│   └── adr/               # アーキテクチャ決定記録 (Architecture Decision Records)
├── .github/
│   ├── ISSUE_TEMPLATE/    # ユーザーストーリー / バグ / タスク
│   ├── workflows/         # CI/CD (GitHub Actions)
│   └── pull_request_template.md
├── CONTRIBUTING.md        # ブランチ戦略・コミット規約・開発フロー
├── SECURITY.md            # セキュリティ・個人情報の取り扱い
└── CHANGELOG.md
```

## 開発の進め方

アジャイル（スクラムベース）で進めます。詳細は以下を参照してください。

- 開発フロー・ブランチ戦略: [CONTRIBUTING.md](CONTRIBUTING.md)
- スプリント運用: [docs/agile/README.md](docs/agile/README.md)
- 技術的な意思決定: [docs/adr/](docs/adr/)

## セットアップ

> 技術スタック確定後に記載します（[ADR](docs/adr/) で決定）。

```bash
# 例:
# git clone <repo-url>
# cd KiraKiraHealth
# <パッケージのインストール>
# <開発サーバー起動>
```

## ライセンス

TBD
