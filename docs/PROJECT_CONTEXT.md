# Project Context: AI Image & Photography Portfolio

このドキュメントは、本プロジェクトの目的、経緯、技術スタック、および今後のロードマップをAIエージェント（Google Antigravity）に共有するためのものです。

## 1. プロジェクト概要
Compassuteの公式ウェブサイトとして、**「AI生成画像」と「実写写真」を中心としたポートフォリオ/ギャラリーサイト**を構築する。

- **リポジトリ名:** `compassute.github.io`
- **サイトの目的:** 作品の展示と作品群のまとめ、および外部プラットフォームへの導線。
- **リポジトリの説明 (Description):** "Portfolio of AI-generated images and photography."

## 2. コンテンツについて
本サイトで扱うメインコンテンツは以下の2軸である。

### A. AI生成画像 (AI Generated Images)
- 本サイトにAI生成画像の作品一覧を掲載する。各画像は販売用より画質を落とし、原則的にwatermarkを付ける。
- **主な生成ジャンル:** 風景
- **使用ツール等の背景:** Lumalabs Dream Machine, Google Whisk, Google Nano Banana, ChaGPT DALL-E, FLUX.1, FLUX.2, SDXL など。

### B. 実写写真 (Photography)
- 本サイトに実写写真の作品一覧を掲載する。各画像は販売用より画質を落とし、原則的にwatermarkを付ける。
- AI作品だけでなく、実写の作品性も重視する。

### C1. 販売先：AI art のデジタル販売
#### 海外向け
- https://aiartshop.com/
- https://gumroad.com/ (スマホ壁紙セット販売)

#### 国内向け
- https://booth.pm

### C2. 販売先：AI art, 実写写真のプリント販売
#### 海外向け
- https://society6.com/

#### 国内向け
- https://suzuri.jp/
- https://www.artgene.net/

### C3. ストックフォト
販売価格が極端に廉価になっているので、あまり乗り気ではないが、結果的に素材向けになってしまった画像はこちらで販売。
#### 海外向け
- https://contributor-accounts.shutterstock.com/
- https://contributor.stock.adobe.com/
- https://wirestock.io/
但し、shutterstockはAI生成画像は禁止であることに注意。

#### 国内向け
- https://pixta.jp/

## 宣伝
- Instagram
- Pinterest

## 3. ウェブサイトの技術スタック & 開発環境
- **プラットフォーム:** GitHub Pages
- **静的サイトジェネレーター:** Jekyll
- **開発エディタ:** Google Antigravity (Local Environment)
- **AIアシスタント:** Gemini 3 (via Antigravity)、ほかにも使用する可能性あり

## 4. 今後のロードマップ (Next Steps)
Antigravity エージェントと共に進めるべきタスクは以下の通り。

- [ ] **環境構築:** ローカルでのJekyll実行環境のセットアップ（Ruby, Bundler等）。
- [ ] **テーマ適用:** サイトのデザインテーマ選定と適用（実写とAI画像が映えるデザイン）。
- [ ] **ページ作成:**
    - Top Page: コンセプトと最新の作品表示。
    - Gallery Page: 作品テーマ群ごとに画像をグリッド等で一覧表示するページ。
    - About Page: Compassuteと活動内容の紹介。
    - 販売先、宣伝先へのリンク集。ギャラリーの各画像から販売先へのリンク以外にリンク集も作成しておく。
- [ ] **デプロイ:** GitHubへのPushとPagesでの公開確認。

## 6. Antigravity エージェントへの特記事項
- ウェブサイトのデザインもimage_creation_preferencesを参考にすること。
- サイト構築においてエラーが発生した場合は、ログを解析し、具体的な修正案または修正コマンドを提示すること。
- デザイン面での提案（例：画像の配置方法、配色の調整）も積極的に行ってほしい。