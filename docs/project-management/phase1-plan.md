---
dest: ./output/project-management/phase1-plan_v1.0.0.pdf
document_title: 組み込みAIソリューション検証プロジェクト
  Phase1実施計画書
---

# Phase1 実施計画書

# 1. 文書概要

本書は、組み込みAIソリューション検証プロジェクトの
**Phase1（環境構築）** における実施計画を整理することを目的とする。

本フェーズでは、AI
SDKを実行するための開発環境を構築し、以降のAI検証フェーズへ移行できる状態を目標とする。

# 2. フェーズ概要

| 項目    | 内容               |
| ----- | ---------------- |
| Phase | Phase1          |
| 名称    | 環境構築 |
| 目的    | AI開発環境を構築し、AI SDKを実行できる状態にする                  |
| 開始予定  |  2026-06                |
| 完了予定  |  2026-07                |

## 2.1 対象WBS

- MS-001～MS-003

## 2.2 リリース成果物

### 動作確認

-   Kakip起動確認
-   DisplayLink表示確認
-   Dockerコンテナ実行環境確認

### ドキュメント

-   README更新
-   概要設計書
-   基本仕様書
-   プロジェクト計画書

### 公開コンテンツ

-   Zenn記事（第1章～第4章）

### GitHub

-   Phase1 Issueクローズ


# 3. プロジェクト体制

| 役割 | 担当 |
|--------|--------|
| プロジェクト責任者 | mono-tec |
| プロジェクトマネージャ | mono-tec |
| 開発担当 | mono-tec |
| テスト担当 | mono-tec |
| ドキュメント作成 | mono-tec |
| AI設計支援 | ChatGPT |
| AIレビュー支援 | ChatGPT |


# 4. QCDS

## 4.1 Quality

-   開発環境構築完了
-   動作確認完了
-   README更新
-   設計書更新

---

## 4.2 Cost（費用）

### 人件費

| 区分 | 金額 |
|--------|--------:|
| --- | TBD |

### AI支援費

| 区分 | 金額 |
|--------|--------:|
| --- | TBD |

### インフラ費

| 区分 | 金額 |
|--------|--------:|
| --- | TBD |

### 諸経費

| 区分 | 金額 |
|--------|--------:|
| --- | TBD |

### プロジェクト総額

| 区分 | 金額 |
|------|------:|
| 人件費 | TBD |
| AI支援費 | TBD |
| インフラ費 | TBD |
| その他 | TBD |
| 合計 | TBD |  

## 4.3 Scope

### 対象

-   Kakipセットアップ
-   DisplayLink環境構築
-   WSL2
-   Ubuntu 24.04
-   Rancher Desktop
-   AI SDK実行環境準備

### 対象外

-   AIサンプル実行
-   USBカメラ接続
-   PLC連携

# 5. スケジュール

``` mermaid
gantt
title Phase1 環境構築
dateFormat YYYY-MM-DD

section 環境構築
MS-001 Kakipセットアップ :a1, 2026-06-27,2d
MS-002 DisplayLink環境構築 :a2, after a1,1d
MS-003 AI開発環境構築 :a3, after a2,3d

section 完了
Phase1 Release :milestone, after a3,0d
```

# 6. 改訂履歴

| 版数     | 改定日 | 内容   |
| ------ | --- | ---- |
| v1.0.0 | 2026-06-30 | 初版作成 |
