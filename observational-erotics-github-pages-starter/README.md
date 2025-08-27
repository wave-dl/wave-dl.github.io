# 観測エロティクス小品集（GitHub Pages / Jekyll）

- Jekyll テーマ: minima
- 日本語フォント: M PLUS 1p Light（`assets/fonts/` に配置でローカル優先）
- コレクション: `stories/`（自由な連作置き場）

## 使い方（GitHub Pages）

1) 新規リポジトリを作成（公開・Public）  
   - 名前を `<username>.github.io` にするとルート運用が簡単。
2) このフォルダ一式をリポジトリにアップロード（`main` ブランチでOK）。  
3) GitHub の Settings → Pages → Build and deployment  
   - Source: `GitHub Actions` か `Deploy from a branch` を選択（`main` / `/ (root)` 推奨）。
4) 数分後、 `https://<username>.github.io/` で公開。

### ローカルでの確認（任意）
Ruby と Bundler がある場合:
```bash
bundle init
bundle add jekyll jekyll-feed jekyll-seo-tag minima
bundle exec jekyll serve
```

### フォントをローカルに置く（任意）
- `assets/fonts/MPLUS1p-Light.ttf` を追加すると、Google Fonts よりローカルフォントが優先されます。

### 新しい短編を追加
- `_posts/YYYY-MM-DD-title.md` を作成（YAML Front Matter に `title` を記載）。

### 連作（storiesコレクション）を追加
- `stories/your-series.md` を作成（Front Matter に `layout: default` と `title`）。