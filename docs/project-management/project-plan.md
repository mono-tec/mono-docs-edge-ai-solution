---
document_title: 組み込みAIソリューション検証プロジェクト_プロジェクト計画書
dest: ./output/project-management/project-plan_v1.1.0.pdf
---

<!-- 表紙 -->
<div class="cover">
  <div class="title">組み込みAIソリューション検証プロジェクト<BR>プロジェクト計画書</div>
  <div class="version">v1.1.0</div>
  <div class="date">2026-06-30</div>
  <div class="logo">

<img
  src="/docs/_shared-images/mono-template.png"
  alt="mono-template"
  width="140"
/>

  </div>
  <div class="copyright">
    © mono-tec Dev
  </div>
</div>

# 1. 文書概要

本書は、組み込みAIソリューション検証プロジェクトの計画を整理することを目的とする。

本プロジェクトでは、エッジAIデバイスを利用したAI推論環境を構築し、設備連携、Web表示、クラウドサービス連携までを段階的に検証する。

また、検証結果をGitHubおよびブログへ公開し、再利用可能な技術資産として蓄積する。

# 2. プロジェクト概要
## 2.1 プロジェクト目的

本プロジェクトでは以下を目的とする。

* エッジAI開発環境の構築
* AI推論環境の構築
* AI推論結果の取得
* 設備機器との連携検証
* Webによる見える化
* クラウドサービスとの連携
* 技術情報の公開および再利用

# 3. コミュニケーション計画

## 3.1 目的

プロジェクト進捗および課題状況を定期的に確認し、
設計・実装・ドキュメント整備を円滑に進める。

## 3.2 コミュニケーション方法

| 項目 | 方法 |
|--------|--------|
| 設計レビュー | ChatGPTとの対話 |
| 技術調査 | ChatGPTとの対話 |
| 実装レビュー | ChatGPTとの対話 |
| 進捗確認 | ChatGPTとの対話 |
| 課題管理 | GitHub Issues またはドキュメント管理 |

## 3.3 レビュータイミング

- 概念設計完了時
- 基本設計完了時
- 内部設計完了時
- 実装完了時
- テスト完了時

# 4. WBS / スケジュール

本書では、プロジェクト全体のWBSを管理する。

各開発フェーズでは、本WBSを基にGitHub Issueを作成し、詳細な作業内容および進捗を管理する。

---

## 4.0 GitHub Labels

GitHub Issueの分類に使用するLabelを定義する。

| Name | Color | Description |
|------|--------|-------------------------------------------|
| phase:design | 6F42C1 | Design and project planning tasks |
| phase:environment | 0E8A16 | Development environment setup tasks |
| phase:ai | FBCA04 | AI verification and model evaluation tasks |
| phase:integration | 1D76DB | System integration and external connectivity tasks |
| phase:release | C5DEF5 | Release and publishing tasks |

---

## 4.1 開発フェーズ

### フェーズ分割方針

本プロジェクトでは、エッジAIソリューションの技術検証を一括で実施するのではなく、検証内容を複数の開発フェーズへ分割して進める。

各フェーズでは、優先度の高い検証から段階的に実施し、動作確認および成果物（設計書、GitHub Issue、Zenn記事等）の整備を行う。

対象WBSは、連続範囲の場合は `MS-001～003`、個別指定の場合は `MS-003,MS-008` の形式で記載する。

| Phase | 名称 | 対象WBS | フェーズ目的 | 計画書 |
| ------ | -------------------- | ---------- | -------------------------- | -------------- |
| Phase1 | 環境構築 | MS-001～003 | KakipおよびAI開発環境を準備する | phase1-plan.md |
| Phase2 | AI検証 | MS-004～006 | AI SDK、USBカメラ、Object Counterを検証する | phase2-plan.md |
| Phase3 | システム連携 | MS-007～009 | Web、PLC、クラウドサービスとの連携を検証する | phase3-plan.md |

---

## 4.2 WBS一覧

※ WBSはプロジェクト全体の管理番号であり、GitHub Issuesおよび各フェーズ実行計画書と対応付けて管理する。

| 管理番号 | GitHub Label | 作業内容 | 期間目安 |
| ------ | -------------------- | -------------------------------- | ---: |
| MS-001 | phase:environment | Kakipセットアップ | 2日 |
| MS-002 | phase:environment | DisplayLink環境構築 | 1日 |
| MS-003 | phase:environment | AI開発環境構築 | 3日 |
| MS-004 | phase:ai | AIサンプル実行 | 2日 |
| MS-005 | phase:ai | USBカメラ接続 | 2日 |
| MS-006 | phase:ai | Object Counter検証 | 3日 |
| MS-007 | phase:integration | Blazorによる見える化 | 3日 |
| MS-008 | phase:integration | Dummy PLC連携 | 2日 |
| MS-009 | phase:integration | クラウドサービス連携 | 3日 |

---

## 4.3 フェーズ締めIssue

各フェーズの完了確認、リリース判断、公開コンテンツの要否判断を行うため、フェーズごとに締めIssueを作成する。

| ID | Phase | タイトル |
|---|---|---|
| REL-001 | Phase1 | Phase1 リリース作業 |
| REL-002 | Phase2 | Phase2 リリース作業 |
| REL-003 | Phase3 | Phase3 リリース作業 |

# 5. 公開方針

## 公開対象

* 技術検証
* 設計書
* サンプルプログラム
* 再現手順
* 技術解説

## 非公開

* 顧客情報
* 実案件情報
* 社内ノウハウ
* 顧客固有設定

# 6. 成功条件

* AI推論が実行できる
* AI結果を取得できる
* 外部システムと連携できる
* GitHub・ブログで再現できる
* 将来の設備向けソリューションへ展開できる

# 7. 今後の展開

* 転移学習
* AI設備監視
* AI外観検査
* AI個数カウント
* Webダッシュボード
* クラウドサービス活用
* 設備向けソリューション化

# 8. まとめ

本プロジェクトでは、組み込みAIを活用した設備向け技術を段階的に検証し、その成果をGitHubおよびブログへ公開する。

設計書・ソースコード・再現手順を技術資産として蓄積し、将来的な設備向けAIソリューションへ展開することを目的とする。

# 9. 改訂履歴

| 版数 | 改定日 | 内容 |
|------|------|------|
| v1.0.0 | 2026-06-27 | 初版作成 | |
| v1.1.0 | 2026-06-30 | GitHubIssu自動作成形式に修正。フェーズ計画書に分割 | |