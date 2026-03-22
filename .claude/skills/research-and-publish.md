---
description: 優先ソースからリサーチして記事を生成しnoteに投稿する
---

# Research & Publish Skill

## 優先リサーチソース（この順番で必ず参照）

| 優先度 | ソース | 用途 |
|--------|--------|------|
| 1 | proceedings.mlr.press | AutoML・ML論文（PMLR） |
| 2 | www.amazon.science | Chronos・AutoGluon-TS時系列論文 |
| 3 | arxiv.org/cs.LG | CS・機械学習論文PDF |
| 4 | ismrepo.ism.ac.jp | 統計数理研究所リポジトリPDF |
| 5 | www.jstage.jst.go.jp | 日本語学術論文PDF |
| 6 | research.facebook.com/publications | Meta AI論文 |
| 7 | zenn.dev | 日本語技術記事 |
| 8 | qiita.com | 日本語技術記事 |

## 実行手順

### STEP 1: リサーチ

ユーザーから【テーマ】を受け取る。
上記優先ソースを順番にweb_fetchで参照し、
関連論文・記事を5件以上収集する。

各ソースから以下を抽出：
- タイトル・URL・要点3行・実装ポイント

### STEP 2: 記事生成

収集情報をもとにnote記事を生成：
- 文体：BT（trendtrap）として実体験ベース・親しみやすく
- 文字数：全体2000文字程度
- 構成：
  ## はじめに
  ## 背景・なぜ重要か
  ## 最新動向（リサーチ結果）
  ## 実践への応用
  ## まとめ
- ハッシュタグ：テーマに応じて自動生成

### STEP 3: note投稿

https://note.com/notes/new にアクセスし
BT（trendtrap）アカウントで下書き保存する。

## 呼び出し方

ユーザーが以下のように指示する：
「@research-publish テーマ：[任意のテーマ]」
