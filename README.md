# .github

`Suki-Suki-Club` オーガナイゼーションのプロフィールリポジトリです。

- `profile/README.md` — [オーガナイゼーションのトップページ](https://github.com/Suki-Suki-Club) に表示されるプロフィール
- `assets/` — プロフィールで使う画像
- `.github/workflows/metrics.yml` — [lowlighter/metrics](https://github.com/lowlighter/metrics) によるリポジトリカードSVG(`repo-*.svg`)の日次自動生成

## セットアップ

統計の全機能を有効にするには、リポジトリシークレット `METRICS_TOKEN` に
classic PAT(`public_repo` + `read:org` スコープ)を登録してください。
未設定でも `GITHUB_TOKEN` にフォールバックして動作します。
