# ドリップノート（デモ）

飲んだコーヒーと味を、1年の文字盤に記録していくデモ。`index.html` 1枚だけで動く。

- 記録はブラウザの localStorage（キー `dripnote-demo.v1`）に保存される。端末・ブラウザごとに別々で、サイトデータを消すと記録も消える。
- ログイン、サーバー、ビルドは不要。
- 写真の登録は未実装（今後追加予定）。

## GitHub Pages で公開する

1. GitHub で新しいリポジトリを作る（例: `dripnote-demo`）。
2. このフォルダで次を実行する。

```bash
git init && git add index.html README.md && git commit -m "Add dripnote demo"
```

```bash
git branch -M main && git remote add origin https://github.com/<ユーザー名>/dripnote-demo.git && git push -u origin main
```

3. リポジトリの Settings → Pages → Branch を `main` / `/ (root)` にして保存。
4. 数分後に `https://<ユーザー名>.github.io/dripnote-demo/` で開ける。

## Vercel で公開する

- GitHub のリポジトリを Vercel に Import する。Framework Preset は「Other」、Build Command と Output Directory は空のままでよい。
- または Vercel CLI で、このフォルダから実行する。

```bash
npx vercel --prod
```
