# kcyf-jp

[KCYF](https://kcyf.jp) コーポレートサイト + [おこっち](https://kcyf.jp/okocchi)アプリ紹介サイト。

KCYF（Keep Connecting Your Family）は「仕事に追われる毎日でも、家族のあたたかさを手放さずにいられる社会へ」をビジョンに、求人マーケティング運用代行と子育て世代向けプロダクト開発を行う個人事業です。本サイトでは KCYF の事業紹介と、初プロダクト「おこっち」（iOS お小遣い管理アプリ）のランディングページ・プライバシーポリシー・利用規約・サポートページを公開しています。

## 🌐 ページ構成

| URL | 内容 |
| :-- | :-- |
| `/` | KCYF コーポレートトップ |
| `/about` | 事業について |
| `/contact` | お問い合わせ |
| `/okocchi` | おこっち アプリ紹介 |
| `/okocchi/privacy` | プライバシーポリシー（App Store 提出用） |
| `/okocchi/terms` | 利用規約（App Store 提出用） |
| `/okocchi/support` | サポート（FAQ・お問い合わせ案内） |
| `/404` | 404 ページ |

## 🛠 技術スタック

- **フレームワーク**: [Astro](https://astro.build/) 6.x（静的サイト生成）
- **CSS**: [Tailwind CSS](https://tailwindcss.com/) 4.x
- **コンテンツ**: MDX（規約類は Markdown を MDX として読み込み）
- **ホスティング**: [Cloudflare Pages](https://pages.cloudflare.com/)
- **ドメイン**: [kcyf.jp](https://kcyf.jp)
- **Node.js**: 20.x 以上

## 🚀 開発コマンド

プロジェクトのルートで実行します。

| コマンド | 動作 |
| :-- | :-- |
| `npm install` | 依存パッケージをインストール |
| `npm run dev` | ローカル開発サーバを `http://localhost:4321` で起動 |
| `npm run build` | 本番ビルド（`./dist/` に出力） |
| `npm run preview` | ビルド結果をローカルでプレビュー |

## ☁️ デプロイ

`main` ブランチへの push をトリガーに、Cloudflare Pages が自動でビルド＆デプロイします。

- **Framework preset**: Astro
- **Build command**: `npm run build`
- **Build output directory**: `dist`

## 📁 ディレクトリ構成

```
kcyf-jp/
├── public/
│   ├── favicon.png
│   └── images/okocchi/        # アプリアイコン・マスコット
├── src/
│   ├── components/            # Header / Footer
│   ├── layouts/               # BaseLayout / DocLayout
│   ├── pages/                 # 各ページ（.astro / .mdx）
│   └── styles/global.css      # Tailwind v4 テーマ定義
├── astro.config.mjs
└── package.json
```

## 📮 お問い合わせ

[support@kcyf.jp](mailto:support@kcyf.jp)

---

© 2026 KCYF
