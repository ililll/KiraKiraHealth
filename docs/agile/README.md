# スプリント運用

## 基本ルール

| 項目 | 内容 |
|------|------|
| スプリント期間 | 1週間〜2週間（チームで決定） |
| バックログ管理 | GitHub Issues + GitHub Projects（カンバン） |
| 見積もり | ストーリーポイント（フィボナッチ: 1, 2, 3, 5, 8, 13） |

## カンバンのステータス

`Backlog` → `Ready` → `In Progress` → `In Review` → `Done`

- `Ready` に入れる条件: [Definition of Ready](definition-of-ready.md)
- `Done` にする条件: [Definition of Done](definition-of-done.md)

## イベント

| イベント | タイミング | 目的 | 記録 |
|----------|------------|------|------|
| スプリントプランニング | スプリント初日 | ゴール設定・バックログ選定 | `docs/sprints/sprint-XX.md` |
| デイリースタンドアップ | 毎日 15分 | 進捗・障害の共有 | 不要 |
| バックログリファインメント | スプリント中盤 | ストーリーの詳細化・見積もり | Issue に追記 |
| スプリントレビュー | スプリント最終日 | 成果物のデモ・フィードバック | `docs/sprints/sprint-XX.md` |
| レトロスペクティブ | スプリント最終日 | プロセス改善 | `docs/sprints/sprint-XX.md` |

## ラベル

| ラベル | 用途 |
|--------|------|
| `story` | ユーザーストーリー |
| `bug` | 不具合 |
| `task` | 技術タスク・スパイク |
| `priority:high` / `priority:medium` / `priority:low` | 優先度 |
| `area:web` / `area:api` / `area:infra` | 対象領域 |
