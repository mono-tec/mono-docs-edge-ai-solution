---
dest: ./output/project-management/phase2-plan_v1.0.0.pdf
document_title: 組み込みAIソリューション検証プロジェクト
  Phase2実施計画書
---

# Phase2 実施計画書

# 1. 文書概要

本書は、組み込みAIソリューション検証プロジェクトの **Phase2（AI検証）**
における実施計画を整理することを目的とする。

# 2. フェーズ概要

| 項目    | 内容               |
| ----- | ---------------- |
| Phase | Phase2          |
| 名称    | AI検証 |
| 目的    | AI SDKおよびAIサンプルを検証し、推論結果を取得する                  |
| 開始予定  |  2026-07                |
| 完了予定  |  2026-07                |

## 2.1 対象WBS

- MS-004～MS-006

## 2.2 リリース成果物

### 動作確認

-   AI SDK動作確認
-   USBカメラ認識
-   Object Counter動作確認

### ドキュメント

-   README更新
-   設計書更新

### 公開コンテンツ

-   Zenn記事（第5章～第7章）

### GitHub

-   Phase2 Issueクローズ

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

-   対象WBS完了
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
title Phase2 AI検証
dateFormat YYYY-MM-DD

section 開発
MS-004 AIサンプル実行 :a1, 2026-07-10,2d
MS-005 USBカメラ接続 :a2, after a1,2d
MS-006 Object Counter検証 :a3, after a2,3d

section 完了
Phase2 Release :milestone, after a3,0d
```
# 6. 改訂履歴

| 版数     | 改定日 | 内容   |
| ------ | --- | ---- |
| v1.0.0 | 2026-06-30 | 初版作成 |
