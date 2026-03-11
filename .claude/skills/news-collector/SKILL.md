---
name: news-collector
description: ニュースを収集してMarkdownにまとめ、アーカイブを管理する
allowed-tools: [web_search, Write, Read, Bash]
---

# News Collector Skill

## 手順

### Step 1: ニュース収集
web_search を使って以下のカテゴリの最新ニュースを収集する。
- AI・テクノロジー
- スタートアップ
- 経済・マーケット

各カテゴリ3〜5件、タイトルと要約（2〜3文）を収集すること。

### Step 2: アーカイブファイルの作成
`docs/archive/YYYY-MM-DD.md` に今日のニュースを保存する。

フォーマット：
```
---
title: YYYY-MM-DD のニュース
date: YYYY-MM-DD
---

# 📰 YYYY-MM-DD のニュース

## 🤖 AI・テクノロジー
- **タイトル**: 要約...
- **タイトル**: 要約...

## 🚀 スタートアップ
- **タイトル**: 要約...

## 📈 経済・マーケット
- **タイトル**: 要約...

## 💡 今日のトレンド考察
全体的なトレンドをまとめた考察...
```

### Step 3: アーカイブ一覧の取得
`Bash` で既存のアーカイブファイルを一覧取得する：
```bash
ls docs/archive/*.md 2>/dev/null | sort -r | head -30
```

### Step 4: index.md の更新
`docs/index.md` を以下のフォーマットで上書きする。
アーカイブ一覧は Step 3 で取得したファイル名から生成すること。

フォーマット：
```
---
title: AI Daily News
---

# 🤖 AI Daily News

> AIが毎日自動収集するニュースまとめ｜最終更新: YYYY-MM-DD

## 🤖 AI・テクノロジー
- **タイトル**: 要約...

## 🚀 スタートアップ
- **タイトル**: 要約...

## 📈 経済・マーケット
- **タイトル**: 要約...

## 💡 今日のトレンド考察
全体的なトレンドをまとめた考察...

---

## 📚 アーカイブ
- [YYYY-MM-DD](archive/YYYY-MM-DD.md)
- [YYYY-MM-DD](archive/YYYY-MM-DD.md)
...（最新30件まで）
```

## 注意事項
- 日付は必ずプロンプトで渡された TODAY の値を使うこと
- アーカイブへのリンクはファイルが存在するものだけを列挙すること
- docs/archive/ ディレクトリが存在しない場合は Bash で作成すること：
  ```bash
  mkdir -p docs/archive
  ```