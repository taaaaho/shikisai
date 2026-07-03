# docs/ — GitHub Pages公開用ディレクトリ

このディレクトリには、App Store Connect登録用のプライバシーポリシー・利用規約ページ(静的HTML)が入っている。

## 公開手順(GitHub Pages)

1. このプロジェクトをGitHubリポジトリにpushする(まだリポジトリ化していない場合は `git init` から)。
2. GitHubのリポジトリ設定 → Pages → Source を「Deploy from a branch」にし、Branch を `main`(または利用するデフォルトブランチ)、フォルダを `/docs` に設定する。
3. 数分後、`https://<ユーザー名>.github.io/<リポジトリ名>/` で公開される。
4. 公開後のURLを確認し、以下に登録する:
   - App Store Connect の「プライバシーポリシーURL」欄 → `.../privacy.html`
   - アプリ内(将来的に設定画面にリンクを追加する場合)

## ファイル構成
- `index.html` — トップページ(サポート情報)
- `privacy.html` — プライバシーポリシー
- `terms.html` — 利用規約
- `style.css` — 共通スタイル(ダークモード対応)

## 更新時の注意
- 各ページの「最終更新日」は内容を変更するたびに手動で更新すること。
- アプリの実装内容(データ保存方法、課金方式など)が変わった場合は、プライバシーポリシー・利用規約の内容も合わせて見直すこと。
