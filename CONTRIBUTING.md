# 開発ガイド (CONTRIBUTING)

## 開発フロー

1. バックログ（GitHub Issues / Projects）からスプリントに取り込まれた Issue を選ぶ
2. Issue に自分をアサインし、ステータスを `In Progress` にする
3. `main` からブランチを作成する
4. 小さくコミットし、Pull Request を作成する（Issue をリンク: `Closes #123`）
5. CI が通り、レビュー承認（1名以上）を得たらマージする
6. [Definition of Done](docs/agile/definition-of-done.md) を満たしたら Issue をクローズ

## ブランチ戦略（GitHub Flow ベース）

- `main` は常にデプロイ可能な状態を保つ
- 作業ブランチは `main` から切り、短命に保つ（目安: 1〜3日でマージ）

| 種類 | 命名規則 | 例 |
|------|----------|----|
| 機能追加 | `feature/<issue番号>-<概要>` | `feature/12-user-signup` |
| バグ修正 | `fix/<issue番号>-<概要>` | `fix/34-login-redirect` |
| 雑務・設定 | `chore/<概要>` | `chore/update-ci` |
| ドキュメント | `docs/<概要>` | `docs/adr-database` |

## コミットメッセージ（Conventional Commits）

```
<type>(<scope>): <概要>

<本文（任意）>

Refs #<issue番号>
```

- `type`: `feat` / `fix` / `docs` / `style` / `refactor` / `test` / `chore` / `ci`
- `scope`: `web` / `api` / `infra` / `docs` など（任意）

例: `feat(api): ユーザー登録エンドポイントを追加`

## Pull Request

- 1 PR = 1 つの目的。大きすぎる場合は分割する（目安: 差分 400 行以内）
- [PR テンプレート](.github/pull_request_template.md) に沿って記載する
- レビュアーは 1 営業日以内にレビューする

## 技術的な意思決定

ライブラリ選定やアーキテクチャに関わる判断は [ADR](docs/adr/) として記録してください。
