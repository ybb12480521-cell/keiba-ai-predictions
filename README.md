# 競馬AI予想 公開サイト

このフォルダは、Windows上の競馬AIアプリから公開用の予想結果だけを書き出す静的サイトです。JV-Link、JRA-VANの利用キー、SQLite DB、学習済みモデルは公開しません。

## 更新

アプリ側でJV-Link取得・特徴量更新・予想を完了した後、プロジェクト直下の `公開サイト更新.ps1` を実行します。`-Push` を付けると、Gitリポジトリ設定済みの場合にコミットとpushまで行います。

```powershell
.\公開サイト更新.ps1
.\公開サイト更新.ps1 -Push
```

公開先では `index.html`、`styles.css`、`app.js`、`predictions.json` だけを配信します。
