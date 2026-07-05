# .github

`Suki-Suki-Club` オーガナイゼーションのプロフィールリポジトリです。

- `profile/README.md` — [オーガナイゼーションのトップページ](https://github.com/Suki-Suki-Club) に表示されるプロフィール
- `assets/` — プロフィールで使う画像
- `.github/workflows/metrics.yml` — [lowlighter/metrics](https://github.com/lowlighter/metrics) によるリポジトリカードSVG(`repo-*.svg`)の日次自動生成。
  公開リポジトリをAPIで自動検出し、カード生成・不要SVGの削除・README のカード一覧
  (`<!-- repo-cards:start/end -->` マーカー区間)の書き換えまで自動で行います

## セットアップ

統計の全機能を有効にするには、リポジトリシークレット `METRICS_TOKEN` に
classic PAT(`public_repo` + `read:org` スコープ)を登録してください。
未設定でも `GITHUB_TOKEN` にフォールバックして動作します。
