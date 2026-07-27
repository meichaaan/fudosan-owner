# 不動産オーナーの資産管理 — 公式サイト

iOSアプリ「不動産オーナーの資産管理」の公式サイト（静的HTML/CSS）です。

**公開URL**: https://meichaaan.github.io/fudosan-owner/

## ページ構成

| ファイル | 内容 | 用途 |
| --- | --- | --- |
| `index.html` | ランディングページ | サイトのトップ |
| `support.html` | サポート | App Store Connect の「サポートURL」 |
| `privacy.html` | プライバシーポリシー | App Store Connect の「プライバシーポリシーURL」 |
| `terms.html` | 利用規約 | アプリ内課金の規約 |
| `tokusho.html` | 特定商取引法に基づく表記 | 課金にあたっての法定表示 |
| `404.html` | 404ページ | GitHub Pages が自動で使用 |

## 構成

- フレームワーク・ビルド不要。HTMLとCSSのみで動きます
- 共通スタイルは `assets/site.css`（`?v=` の数字はキャッシュ対策。**CSSを変更したら全HTMLのバージョンを揃えて上げること**）
- アプリのスクリーンショットは `assets/shot-*.jpg`
- SNSシェア用のカード画像は `assets/og-card.jpg`（1200×630）

## ローカルで確認する

```bash
python3 -m http.server 8930
```

http://localhost:8930 を開きます。

## 更新のしかた

ファイルを編集して push すると、1〜2分で公開サイトに反映されます。

```bash
git add -A && git commit -m "更新内容" && git push
```

## 残っているTODO

- App Store 公開後、`index.html` 内の `.store-badge`（2箇所）のリンクを実際のApp Store URLに差し替える
- 独自ドメインを設定する場合は、各ページの `og:url` / `canonical`、`robots.txt`、`sitemap.xml` のURLも差し替える

---

© 2026 合同会社K's Casa
