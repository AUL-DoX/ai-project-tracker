以下をそのまま **README.md** として使える。
GitHub公開を想定した構成にしてある。

---

# AI Development Project Manager

AIツール（ChatGPT / Claude / Gemini）を使って作ったプロジェクトを
ブラウザだけで管理できるシンプルな管理アプリです。

インストール不要。
HTMLファイルを開くだけで動作します。

ローカルストレージを使用してデータを保存するため、
外部サーバーへのデータ送信はありません。

---

# Overview

AIを使って開発をしていると、

* 作ったツールが増える
* どのAIで作ったか忘れる
* GitHub / デモ / Chat URL がバラバラになる

という問題が起きます。

このツールはそれらを **1ページで管理するための軽量アプリ** です。

---

# Features

* プロジェクト登録
* AI種別管理

  * ChatGPT
  * Gemini
  * Claude
* プロジェクト説明メモ
* タグ管理
* URLリンク管理
* 検索機能
* AI別フィルター
* 統計表示
* JSONエクスポート
* JSONインポート

すべて **ブラウザ内で完結** します。

---

# How It Works

このアプリは次の技術で作られています。

* HTML
* CSS
* Vanilla JavaScript
* LocalStorage

バックエンドやデータベースは使用していません。

データはブラウザの **LocalStorage** に保存されます。

---

# Usage

### 1. プロジェクトを登録

フォームに入力します。

* プロジェクト名
* 使用AI
* 開発日
* 説明
* タグ
* 関連URL

「プロジェクトを追加」を押すと保存されます。

---

### 2. プロジェクトを管理

カード形式で一覧表示されます。

可能な操作

* 編集
* 削除
* URLリンクを開く

---

### 3. 検索

検索ボックスから

* プロジェクト名
* 説明
* タグ

を検索できます。

---

### 4. フィルター

AIごとに表示を切り替えできます。

* All
* ChatGPT
* Gemini
* Claude

---

### 5. データバックアップ

データはJSON形式で保存できます。

Export
→ JSONファイルをダウンロード

Import
→ JSONを読み込んで復元

---

# Data Storage

保存先

```
LocalStorage
key: aiProjects
```

ブラウザ内にのみ保存されます。

そのため

* 他のPCには同期されません
* ブラウザ削除でデータも消えます

必要な場合は **JSON Export** を使用してください。

---

# Installation

このプロジェクトはビルド不要です。

```
git clone
```

または

```
Download ZIP
```

その後

```
index.html
```

をブラウザで開くだけで動作します。

---

# Security & Privacy

このアプリは

* 外部サーバー通信なし
* ユーザーデータ送信なし
* ローカル保存のみ

の設計です。

---

# Possible Future Improvements

* お気に入り機能
* カテゴリ管理
* ダッシュボード化
* AIランチャー機能
* GitHubリンク統合

---

# License

MIT License

---

# Author

AUL DoX

AI開発・DXツール研究プロジェクト

も作れる。
実は今のREADMEは「技術者向け」で、GitHubでは少し改良するとかなり見栄えが良くなる。
