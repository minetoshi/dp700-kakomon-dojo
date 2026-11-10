# DP-700 学習コンテンツ品質基準（2026-10-19版）

基準: https://learn.microsoft.com/ja-jp/credentials/certifications/resources/study-guides/dp-700

## 必須チェック

- 公式ガイドの評価項目に各問題を紐付ける（domain / objective / subskill）。
- 問題文、正答、全選択肢の解説、公式根拠リンクを検証する。
- 正答が一意か、Fabric の現行仕様と整合するか、古い名称・廃止機能がないかを確認する。
- 解説は「正解理由」と「誤答理由」を明記する。実際の試験問題の転載・流出問題は取り込まない。
- 3分野を各30–35%の目安でカバーする。設問数の配分だけでなく、全サブスキルのカバーを優先する。
- 難易度、コード読解（SQL / PySpark / KQL）、シナリオ問題、障害調査問題を別途点検する。
- 設問の状態を未監査 / 要修正 / 検証済みで管理し、未検証の正確性を保証しない。

## 公式分野

1. 分析ソリューションの実装と管理（30–35%）: Spark / domain / OneLake / Airflow workspace settings、version control、database projects、deployment pipelines、workspace / item / granular access、masking、sensitivity labels、endorsement、audit logs、OneLake security、Dataflow Gen2 / pipeline / notebook、triggers、parameters / expressions。
2. データの取り込みと変換（30–35%）: full / incremental / streaming loads、dimensional models、store selection、shortcuts、mirroring、pipeline、PySpark / SQL / KQL、deduplication / late arrivals、Eventstream、Spark structured streaming、window functions。
3. 分析ソリューションの監視と最適化（30–35%）: ingestion / transformation / semantic refresh monitoring、alerts、pipeline / Dataflow Gen2 / notebook / Eventhouse / Eventstream / T-SQL / shortcut errors、Lakehouse / pipeline / warehouse / real-time / Spark / query performance。

## 既存サイトで確認したこと

- `index.html` の画面には「オリジナル模擬問題・全90問」と表示される。
- この文書の追加は既存90問の個別正誤検証を意味しない。設問の全件レビューと採点は未完了。

## 外部教材の統合候補

- 原著: https://github.com/kengio/dp-700-study-guide
- 82 practice + 3 × 50 mock = 232 questions。原著は2026-07-21版に基づくため2026-10-19版との突合が必要。
- MIT License。翻訳物にも原著著作権表示とLICENSE全文を同梱し、原典・改変の旨を表示する。
- 既存のオリジナル問題と別バンクで管理し、問題IDの衝突を避ける。
- 翻訳時には技術語（Lakehouse、Eventhouse、OneLake shortcut、KQLなど）の意味を保持し、選択肢と解説を照合する。
- 未翻訳・未検証問題を日本語版として公開しない。公開前に各問の選択肢・正答・解説の整合性を検証する。

## 次の実装タスク

1. 既存90問の問題ID・公式subskill対応表を生成し、カバレッジと誤りを監査。
2. 原著232問のデータ形式を確認し、日本語版の別バンクへ移植。
3. 全232問の翻訳・用語統一・正答検証、MIT表記を実装。
4. GitHub Pagesで切替、出題、採点、進捗保持、スマホ表示を検証。
