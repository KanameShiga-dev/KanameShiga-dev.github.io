# 情報漏洩ビンゴ 2026秋

2026年9月1日〜10月9日に国内で公表された情報漏洩39件から、毎回24件を引いて作るビンゴカードです。

- マスをタップすると「漏」の判が押され、公表日・件数・状況・公表元リンクが表示されます
- 中央は FREE（お詫びとお知らせ）
- 「新しいカード」で引き直し、「印を消す」でリセット
- 印の状態はブラウザの localStorage に保存されます

## 公開方法（GitHub Pages）

このフォルダを既存の `KanameShiga-dev.github.io` リポジトリの `leak-bingo/` に配置します。既存サイトの Pages 設定を使い、公開先は `https://kanameshiga-dev.github.io/leak-bingo/` です。

依存ファイルなし。フォントのみ Google Fonts から読み込みます。

## データについて

- 件数は各社公表値の上限で、「漏えい確定」と「漏えいのおそれ」が混在します。全件流出を意味しません
- 主な集計出典：[セキュリティ対策Lab「2026年9〜10月の主要案件で延べ1億件相当超」](https://rocket-boys.co.jp/security-measures-lab/2026-sep-oct-japan-data-breach-exposure-scale/) ほか各社公表資料
- データ更新は `index.html` 内の `POOL` 配列を編集してください（`ok:1` = 漏えい確認、`ok:0` = おそれ・可能性）

データ時点：2026年10月16日
