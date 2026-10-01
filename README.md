# Shoma Yamamoto (@6plusjp)

**TypeScript / Rust / React / Remix を用いたフルスタック開発・ブラウザ拡張・CLI ツールの自作実績あり**  
稼働中ポートフォリオ: https://6plus.vercel.app

---

## Projects

### [www_vercel](https://github.com/6plusjp/www_vercel) — ポートフォリオサイト（本番稼働中）
Remix + Vite + TypeScript + Tailwind CSS + MDX で構築した SSR デプロイのポートフォリオサイト。

- **ルーティング**: 20ルート（ブログ / 実績 / 履歴書〈日英切替・PDF生成〉 / 問い合わせ / ポリシー / RSS / API エンドポイント）
- **テスト**: Playwright による E2E テスト
- **デプロイ**: Vercel（SSR）
- **コードベース**: TS/TSX/CSS 約 8,200 行、372 commits（2022-04 より継続）

**技術的特色**  
Remix のローダー/アクションを活用したサーバーサイドレンダリング、MDX ベースのコンテンツ管理、動的 OG 画像生成、多言語対応（i18n）を自前で実装。

---

### [protonvpn-tui](https://github.com/6plusjp/protonvpn-tui) — ProtonVPN 用ターミナル UI（Rust）
`protonvpn-cli` をラップし、国・都市の階層ブラウズ・ファジー検索・テーマ切替・接続セッション管理を提供する TUI アプリケーション。

- **アーキテクチャ**: `vpn` / `ui` / `state` / `config` の 4 モジュールに明確分離
- **品質保証**: GitHub Actions CI、`clippy.toml` / `rustfmt.toml` による静的解析、統合テスト 7 本
- **ドキュメント運用**: 解決済み Issue 112 本を `docs/issue/` に記録（根本原因と解決策を体系化）、`docs/policy/` にコーディング規約 5 種
- **ライセンス**: MIT、README 227 行と設計ドキュメント完備

**技術的特色**  
非同期ランタイム、ステートマシンによる接続状態管理、設定の型安全な永続化、クロスプラットフォーム対応（Linux/macOS）を Rust の型システムで担保。

---

### [vimora](https://github.com/6plusjp/vimora) — Firefox 向け Vim 風ブラウザ拡張（Manifest V3）
Vim 風モード（normal / insert / hint / visual / omni / find 等）を提供する Firefox 拡張。

- **アーキテクチャ**: Clean Architecture による層分離（core は副作用なし・純粋関数）
- **テスト**: Playwright E2E 19 本 + Vitest ユニット/統合 36 ファイル
- **フレームワーク**: WXT + TypeScript

**技術的特色**  
Manifest V3 の制約下で Service Worker 型バックグラウンドスクリプトと Content Script 間のメッセージングを型安全に実装、キーマッピングエンジンをコアロジックとして切り出しテスタビリティを確保。

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| **Languages** | TypeScript, Rust, Python, JavaScript |
| **Frontend** | React, Remix, Next.js, Tailwind CSS, MDX |
| **Testing** | Playwright, Vitest |
| **Browser Extension** | WXT (Firefox MV3) |
| **CLI / TUI** | Rust (ratatui, clap, tokio) |
| **Infrastructure** | Vercel, GitHub Actions |

---

## Development Environment

- **OS**: Arch Linux（自作 dotfiles で Provisioning・標準化）
- **Editor**: Neovim（LSP / Treesitter / デバッガー統合）
- **Shell**: Fish（カスタム補完・プロンプト・エイリアス）
- **Window Manager**: Hyprland（Wayland・タイル型）
- **Dotfiles**: 全設定をコード化し、新環境への展開を自動化

---

## Contact

- GitHub: [@6plusjp](https://github.com/6plusjp)
- Portfolio: [6plus.vercel.app](https://6plus.vercel.app)
- Email: （必要に応じて記載）

---

> すべて個人制作・独学による成果物です。実務経験としての主張は含みません。