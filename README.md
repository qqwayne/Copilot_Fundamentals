# Copilot Fundamentals - デモ

このリポジトリは、Copilot の機能を示すサンプルとツールをいくつか収めています：

- `demos/copilot-essentials`：基本的なユーティリティ（例：ログ解析ツール `triage.py`）
- `demos/copilot-agents`：Copilot Agents のワークフローを示すデモ（`ISSUE.md`、`STEER.md`、`README.md` を含む）

## クイックスタート

1. デモの説明を確認：
   - `demos/copilot-agents/README.md` — Copilot Agents デモの手順とサンプル Issue
   - `demos/copilot-essentials/README.md` — `triage` ツールの簡単な説明（存在する場合）

2. `triage.py` を実行する（例）
   - 要件：Python 3.8+
   - コマンド例：
     ```zsh
     python3 demos/copilot-essentials/triage.py --file ./demos/copilot-essentials/sample_access.log.gz --minutes 15 --status 499,321 --top 10
     ```
   - 説明：スクリプトは `.log` と `.log.gz` をサポートし、直近 N 分間のスライディングウィンドウで (status, path) ペアを集計して上位 N 件を出力します。

3. Copilot Agents デモを実行する
   - `demos/copilot-agents/ISSUE.md` の Title と Body をコピーして新しい GitHub Issue を作成し、Copilot に割り当ててエージェントタスクを開始してください
   - セッション中に `demos/copilot-agents/STEER.md` を貼り付けて要件を変更できます

## リポジトリ構成（概要）

```
demos/
  copilot-agents/
    ISSUE.md
    README.md
    STEER.md
  copilot-essentials/
    triage.py
    sample_access.log.gz
    README.md
```

## 貢献ガイド

サンプルやドキュメントを改善したい場合は PR を送ってください。変更の目的と検証手順を説明に含めてください。
