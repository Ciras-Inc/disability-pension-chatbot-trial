# disability-pension-chatbot-trial｜リポジトリ固有情報

対象：`Ciras-Inc/disability-pension-chatbot-trial`。既存のAI入口がないため、実在する構成・コマンドと依頼内容から作業範囲を確認する。未確認の用途や公開先を推測しない。

## 今回照合した構成

- 既定branch：`main`
- 配布前commit：`e7a26694d41ac50a9d6bc30d3c703ba0578c2cc4`
- 既存lockfile：rootでは未確認
- 必須status check：取得できたRuleset内には指定なし。従来型branch protectionの不存在を意味しない

検査候補は `.ciras/ai-profile.json` の `local_check_commands` を参照。既存宣言を読み取った一覧であり、今回すべてを実行した結果ではない。依存関係・外部効果・実行面を確認して必要なものを使う。パッケージ管理を他repoの方式へ一律変更しない。
