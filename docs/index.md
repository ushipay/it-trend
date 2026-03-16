---
title: IT Trend Daily
---

# 💻 IT Trend Daily

> AIが毎日自動収集するITトレンドニュース｜最終更新: 2026-03-16

## 🤖 AI・機械学習

- **[政府AI基盤「源内」、18万人対象の実証開始 国産LLM7モデル選定](https://www.itmedia.co.jp/enterprise/articles/2603/11/news042.html)**: デジタル庁は政府職員約18万人を対象とする生成AI基盤「ガバメントAI（源内）」の大規模実証を開始。NTTグループの「tsuzumi 2」、ソフトバンクの「Sarashina2 mini」など国産LLM7モデルを選定し、2026年5月から全府省庁に展開する。

- **[GitHub、Claude・CodexのAIエージェントをプラットフォームに統合](https://www.techbuzz.ai/articles/github-opens-platform-to-claude-and-codex-ai-agents)**: GitHubが「Agent HQ」を立ち上げ、AnthropicのClaudeとOpenAIのCodexをGitHub・VS Code上のワークフローに統合。Copilot Pro Plus・Enterpriseユーザーがパブリックプレビューで利用可能となり、67%の開発者がAIツールを日常的に活用するまでに普及が拡大している。

- **[GitHub Copilot学生プランからClaudeプレミアムモデルが削除](https://www.theregister.com/2026/03/13/microsoft_github_removes_models_student_plan/)**: 2026年3月12日、GitHubはCopilot学生プランの再編に伴い、Claude Opus・Sonnet・GPT-5.4の手動選択を廃止。コスト維持の問題を理由に挙げたが、コミュニティで1,836件のダウンボートと激しい反発を招いた。

- **[Gartnerが「ドメイン特化型LLM」を今後5年の重要技術トレンドに選定](https://www.itmedia.co.jp/aiplus/articles/2601/30/news032.html)**: Gartnerは2027年までに企業利用の生成AIモデルの50%以上が特定業界・業務に特化すると予測。汎用LLMよりも高い正確性と信頼性を持つドメイン特化型言語モデル（DSLM）への移行が加速する見込み。

- **[LLM・SLM・フロンティアモデルの使い分けが重要トレンドに](https://blogs.itmedia.co.jp/osonoi/2026/03/aillmslm.html)**: 大規模LLMですべてを解決するのではなく、適材適所でAIモデルを組み合わせる「マルチモデル戦略」が広まりつつある。LLMは文脈理解、フロンティアモデルは高度推論・AIエージェント用途に特化し、コスト・性能を最適化するアプローチが注目されている。

## ☁️ クラウド・インフラ

- **[AzureのMCP Server脆弱性（CVE-2026-26118）が修正](https://www.helpnetsecurity.com/2026/03/11/march-2026-patch-tuesday/)**: 3月のPatch TuesdayでAzure Model Context Protocol（MCP）サーバーにCVSSスコア8.8のSSRF脆弱性が修正された。攻撃者がユーザー提供パラメータを受け取るツールへ特細工された入力を送ることで、マネージドIDの権限昇格が可能となる危険性があった。

- **[クラウド市場：AWSシェアが30%を割り込み、Azureが着実に成長](https://www.publickey1.jp/blog/25/aws30azure2220251synergy_research.html)**: 2025年第1四半期のSynergy Research調査によると、AWSのクラウドシェアがついに30%を下回った。Azureは22%と着実に成長しており、AI戦略（Azure OpenAI Service・Copilot連携）が企業顧客獲得を後押ししている。

- **[クラウド市場は2034年に5兆1500億ドル規模へ拡大予測](https://zenn.dev/milmed/articles/edee5b170fa652)**: Precedence Researchの調査によると、世界のクラウド市場は生成AIの爆発的成長を背景に、2025年の9,128億ドルから2034年には5兆1,509億ドルへ成長する見込み。ハイパースケーラー各社はAIインフラへの投資を拡大しており、2025年通年で19%の市場成長が予測されている。

- **[GCPのVertex AIが機械学習プラットフォームとして評価向上](https://cloud.google.com/docs/get-started/aws-azure-gcp-service-comparison?hl=ja)**: Google CloudのVertex AIが、機械学習モデルの開発から本番運用までワンストップで対応するプラットフォームとして評価を高めている。TensorFlowとの高い親和性やBigQueryなどデータ分析ツールとの連携が強みで、AI開発用途でのGCP採用が増加している。

## 🛠️ ソフトウェア開発

- **[IPA「Japan Open Source Hub」がOSS推進の最新成果を公開](https://www.ipa.go.jp/digital/kaihatsu/oss/index.html)**: IPAは2026年3月10日に「OSPOレベル1構築ワークショップ」成果発表会を公開。3月4日には「行政によるOSS公開活動の国際比較調査報告書」も公開し、日本のOSS活用促進に向けた施策を強化している。

- **[RAGとLLMの連携：「DRAMからの脱却」というパラダイムシフト](https://eetimes.itmedia.co.jp/ee/articles/2603/02/news005.html)**: 「社会知識（データ）と知能（LLMの処理）を分離し、LLMには"考える能力"に集中させる」設計思想が広まりつつある。RAGとベクターデータベースの積極的活用により、LLMのデータ量限界という課題を克服するアーキテクチャが実用化段階に入っている。

- **[MCP（Model Context Protocol）がAI開発の業界標準として定着](https://qiita.com/aokikenichi/items/fca5a1898cc2a9c961f6)**: Anthropic社が2024年11月に発表したMCPは、各種APIを一括で扱える「マルチアダプター」として機能し、OpenAI・Google・Amazonも採用を発表。MCPを活用した自律型ペネトレーションテストツール「PentestMCP」など、多様な活用事例も登場している。

- **[DeNA、LLM勉強会資料とコードを全公開](https://www.itmedia.co.jp/aiplus/articles/2512/05/news086.html)**: DeNAの「AIエンジニアが本気で作った」LLM学習用資料とコードがオープンソースで公開された。非エンジニアでも学べる内容になっており、企業内でのAI・LLMリスキリング促進に貢献することが期待されている。

## 🔒 セキュリティ

- **[Microsoft 2026年3月Patch Tuesday：84件の脆弱性を修正、2件のゼロデイ対応](https://thehackernews.com/2026/03/microsoft-patches-84-flaws-in-march.html)**: 3月10日にMicrosoftが84件の脆弱性を修正するセキュリティアップデートをリリース。うち8件がCritical評価で、2件のゼロデイ脆弱性（CVE-2026-26127：.NETのDoS、CVE-2026-21262：SQL Serverの権限昇格）も修正された。即時適用が推奨されている。

- **[Windowsカーネル・SMBサーバーに悪用可能性の高い権限昇格脆弱性](https://www.bleepingcomputer.com/news/microsoft/microsoft-march-2026-patch-tuesday-fixes-2-zero-days-79-flaws/)**: 今月のPatch Tuesdayでは、Windowsカーネルの解放後使用（Use-after-free）脆弱性、Windowsグラフィックスコンポーネントの競合状態、SMBサーバーの認証不備など6件が「悪用される可能性が高い」として特に注意が促されている。

- **[Microsoft Authenticatorにフィッシング・MitM攻撃リスク（CVE-2026-26123）](https://krebsonsecurity.com/2026/03/microsoft-patch-tuesday-march-2026-edition/)**: CVE-2026-26123がAndroid・iOS向けMicrosoft Authenticatorに影響し、攻撃者が不正アプリを介してサインイン情報を中間者攻撃で取得できる可能性がある。高度な技術を持つ攻撃者による標的型攻撃での悪用が懸念される。

- **[AIを悪用したサイバー攻撃がより高速・高度化：トレンドマイクロ脅威予測](https://www.trendmicro.com/ja_jp/research/26/c/the-march-2026-security-update-review.html)**: 攻撃者はAIを活用して攻撃プロセスを自動化し、高度なソーシャルエンジニアリングを生成。AI推論システム（CRS）の普及により、ゼロデイ攻撃の実行速度と脆弱性発見範囲が拡大しており、防御側もAIを活用した対策が急務となっている。

- **[IPA「情報セキュリティ10大脅威 2026」公表](https://www.ipa.go.jp/security/10threats/10threats2026.html)**: IPAが「情報セキュリティ10大脅威 2026」を決定・公表し、組織編の解説書も公開。ランサムウェア、サプライチェーン攻撃、AIを悪用した攻撃などが引き続き主要脅威として挙げられている。

## 💡 今日のITトレンド考察

2026年3月16日時点のITトレンドを俯瞰すると、**「AIの社会実装フェーズへの本格移行」**が最大のテーマとして浮かび上がる。

日本では政府AI基盤「源内」での国産LLM大規模実証開始が象徴的で、AI活用が「実験」から「業務運用」へと転換する転換点を迎えている。一方、GitHubがClaude・Codexをプラットフォームに統合したことは、開発者ツール領域での**「マルチモデルAI時代」**の到来を示しており、単一AIベンダーへの依存から脱却する動きが加速している。

クラウド分野では、AWSのシェア低下とAzureの成長が続く中、各社のAI戦略の優劣がシェア変動を左右する重要因子となっている。セキュリティ面では、84件の脆弱性を修正した3月Patch TuesdayやAIを悪用したサイバー攻撃の高度化が示すように、攻守両面でのAI活用が急務となっている。エンジニアには、AIの恩恵を享受しながらも、AIが新たなリスク要因にもなりうるという二重の視点が求められる時代となった。

---

## 📚 アーカイブ

- [2026-03-16](archive/2026-03-16.md)
- [2026-03-15](archive/2026-03-15.md)
- [2026-03-14](archive/2026-03-14.md)
- [2026-03-13](archive/2026-03-13.md)
- [2026-03-12](archive/2026-03-12.md)
