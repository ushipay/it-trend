---
name: news-collector
description: ITトレンドニュースを収集してMarkdownにまとめ、アーカイブを管理する
allowed-tools: [web_search, Write, Read, Bash]
---

# IT Trend News Collector Skill

## 手順

### Step 1: ニュース収集
web_search を使って以下のカテゴリのIT関連最新ニュースを収集する。
- AI・機械学習（LLM、生成AI、MLOps、AI開発ツールなど）
- クラウド・インフラ（AWS/Azure/GCP、コンテナ、サーバーレス、DevOpsなど）
- ソフトウェア開発（プログラミング言語、フレームワーク、開発手法、OSS など）
- セキュリティ（脆弱性、サイバー攻撃、セキュリティツール、規制動向など）

各カテゴリ5〜10件、タイトルと要約（2〜3文）、および参照元のURLを収集すること。
IT業界のエンジニア・開発者にとって実用的で価値のある情報を優先すること。

#### 優先ソース
以下のサイトを優先的に情報源として使用すること。他のソースも排除はしないが、
信頼性・専門性の高いこれらのサイトからの情報を優先する。

**日本語サイト：**
- Publickey（https://www.publickey1.jp/） - クラウド・インフラ・開発ツール
- ITmedia NEWS（https://www.itmedia.co.jp/news/） - IT業界全般
- @IT（https://atmarkit.itmedia.co.jp/） - エンジニア向け技術解説
- Zenn（https://zenn.dev/） - 開発者コミュニティのトレンド
- Qiita（https://qiita.com/） - エンジニアの技術共有
- gihyo.jp（https://gihyo.jp/） - 技術評論社の技術記事
- クラウドWatch（https://cloud.watch.impress.co.jp/） - クラウド・インフラ専門
- piyolog（https://piyolog.hatenadiary.jp/） - セキュリティインシデント

**英語サイト：**
- Hacker News（https://news.ycombinator.com/） - テック業界の最新話題
- InfoQ（https://www.infoq.com/） - ソフトウェア開発の深い技術記事
- TechCrunch（https://techcrunch.com/） - テック企業・プロダクト
- The Hacker News（https://thehackernews.com/） - セキュリティ専門
- GitHub Blog（https://github.blog/） - OSS・開発ツール
- Dev.to（https://dev.to/） - 開発者コミュニティ

### Step 2: アーカイブファイルの作成
`docs/archive/YYYY-MM-DD.md` に今日のニュースを保存する。

フォーマット：
```
---
title: YYYY-MM-DD のITトレンド
date: YYYY-MM-DD
---

# 💻 YYYY-MM-DD のITトレンド

## 🤖 AI・機械学習
- **[タイトル](URL)**: 要約...
- **[タイトル](URL)**: 要約...

## ☁️ クラウド・インフラ
- **[タイトル](URL)**: 要約...

## 🛠️ ソフトウェア開発
- **[タイトル](URL)**: 要約...

## 🔒 セキュリティ
- **[タイトル](URL)**: 要約...

## 💡 今日のITトレンド考察
IT業界全体のトレンドをまとめた考察（技術の方向性、エンジニアへの影響など）...
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
title: IT Trend Daily
---

# 💻 IT Trend Daily

> AIが毎日自動収集するITトレンドニュース｜最終更新: YYYY-MM-DD

## 🤖 AI・機械学習
- **[タイトル](URL)**: 要約...

## ☁️ クラウド・インフラ
- **[タイトル](URL)**: 要約...

## 🛠️ ソフトウェア開発
- **[タイトル](URL)**: 要約...

## 🔒 セキュリティ
- **[タイトル](URL)**: 要約...

## 💡 今日のITトレンド考察
IT業界全体のトレンドをまとめた考察...

---

## 📚 アーカイブ
- [YYYY-MM-DD](archive/YYYY-MM-DD.md)
- [YYYY-MM-DD](archive/YYYY-MM-DD.md)
...（最新30件まで）
```

## 注意事項
- 日付は必ずプロンプトで渡された TODAY の値を使うこと
- 各ニュース項目のタイトルには必ず参照元のURLをMarkdownリンクとして付与すること（`**[タイトル](URL)**` の形式）
- アーカイブへのリンクはファイルが存在するものだけを列挙すること
- docs/archive/ ディレクトリが存在しない場合は Bash で作成すること：
  ```bash
  mkdir -p docs/archive
  ```