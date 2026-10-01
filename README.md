# Shoma Yamamoto (@6plusjp)

**TypeScript / Rust を用いた Web アプリケーション開発・CLI ツールの自作プロジェクト**<br>
稼働中ポートフォリオ: https://6plus.vercel.app

---

## Projects

### [www_vercel](https://github.com/6plusjp/www_vercel) — ポートフォリオサイト（本番稼働中）
Remix + Vite + TypeScript + Tailwind CSS + MDX で構築した SSR デプロイのポートフォリオサイト。

- **ルーティング**: 20ルート（ブログ / 実績 / 履歴書〈日英切替・PDF生成〉 / 問い合わせ / ポリシー / RSS / API エンドポイント）
- **テスト**: Playwright による E2E テスト
- **デプロイ**: Vercel（SSR）
- **コードベース**: TS/TSX/CSS 約 8,000 行、20 ルート、2022-04 より継続的に開発

**技術的特色**  
Remix の loader / action を活用したサーバーサイドレンダリング、MDX ベースのファイルベースコンテンツ管理、OG メタタグの一元管理、履歴書の `$lang` パラメータによる言語切替と PDF 生成。Vercel のビルド出力と ESM/CJS 混在の実務的な解決。

---

### [protonvpn-tui](https://github.com/6plusjp/protonvpn-tui) — ProtonVPN 用ターミナル UI（Rust）
`protonvpn-cli` をラップし、国・都市の階層ブラウズ・ファジー検索・テーマ切替・接続セッション管理を提供する TUI アプリケーション。

- **アーキテクチャ**: `vpn` / `ui` / `state` / `config` の 4 モジュールに明確分離
- **品質保証**: GitHub Actions による自動テスト、`clippy.toml` / `rustfmt.toml` による静的解析・フォーマット規約、統合テスト 5 本
- **ドキュメント運用**: 解決済み Issue の記録 107 件を `docs/issue/` に蓄積（根本原因と解決策を体系化）、`docs/policy/` にコーディング規約 6 種
- **開発期間**: 2026-03 〜 2026-10 の約 7 か月間、Rust ソース約 12,000 行
- **ライセンス**: MIT、設計ドキュメントと Issue 運用記録を完備

**技術的特色**  
`ratatui` / `crossterm` による TUI レンダリング、`thiserror` による型安全なエラーハンドリング、`serde` + `toml` による設定の永続化。接続状態をステートマシンとして管理し、CLI との非同期なやり取りをイベント駆動で処理。

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| **Languages** | TypeScript, Rust, Python, JavaScript |
| **Frontend** | React, Remix, Next.js, Tailwind CSS, MDX |
| **Testing** | Playwright, Vitest |
| **CLI / TUI** | Rust (ratatui, crossterm, clap, serde) |
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