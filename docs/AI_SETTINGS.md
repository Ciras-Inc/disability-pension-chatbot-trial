# AI設定 CIRAS-SUCCESS-20261028-R2.1

共通入口は[AGENTS.md](../AGENTS.md)、Claude Codeは[CLAUDE.md](../CLAUDE.md)、CursorはAGENTSと常時適用ルールを使用します。固有の技術条件・コマンドは[repository-context.md](../.ciras/repository-context.md)を参照します。

## 配布版

- 正本：Ciras-Inc/ciras-os の commit `c5314f29f2ee7706f3d553f6695840d9a05608ae`
- 生成器：`1.0.0`
- 対象：`Ciras-Inc/disability-pension-chatbot-trial`
- 既定branch：`main`
- 配布台帳：`.ciras/governance-release.yaml`
- 出力照合：`.ciras/ai-settings-manifest.json`

## 確認と更新

`node .ciras/verify-ai-settings.mjs --root .` で構成・hashを確認します。最終配布検査は固定元の検査器と別に固定したmanifest hashを使います。候補内の検査器・hashだけでは承認や改ざん耐性の証拠になりません。

設定更新は作業branchとPRで行い、共通規則は固定元の生成器から再生成します。既存の必須チェック・レビュー・本人実行条件を守ります。既存の権限、hook、sandbox、Ruleset、共有・課金設定はこの配布で変更しません。

## 実行面の状態

この配布はファイル構成の検査です。Claude Code・Cursor・Codexの実製品での読込、trust、権限、許可/拒否の動作は未検証です。各実行面で確認し、未検証の危険操作は保留、独立した通常作業は継続します。新規native権限・MCP・hookを空の設定で上書きしません。

## 復元

配布前commitは `e7a26694d41ac50a9d6bc30d3c703ba0578c2cc4`。適用済みPRを取り消す場合は対象差分を確認した追加のrevert PRで戻します。force pushや既存履歴の書換えは行いません。
