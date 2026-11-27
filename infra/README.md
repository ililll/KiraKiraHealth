# infra

インフラ構成（IaC）を配置します。

```
infra/
├── modules/        # 再利用可能なモジュール
└── envs/
    ├── dev/
    ├── staging/
    └── production/
```

クラウド・IaC ツールの選定は ADR で決定します。
