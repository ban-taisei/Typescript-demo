今回はTypeScriptのチュートリアルを行いました。
「サバイバルTypeScript」を基に、実際に手を動かすことで体験しました。https://typescriptbook.jp/tutorials


内容
- 開発環境の準備
    Node.jsのインストール
  　TypeScriptのインストール
- 簡単な関数を作ってみよう
  　JavaScriptをTypeScriptに変換する
  　コンパイラを動かす
- Reactでいいねをボタンを作ろう
  　Reactとは？
  　Reactの3大特徴
  　プロジェクトを作る
  　ボタンを作る場所を用意する
  　ボタンのビジュアルを作り込む
  　ボタンに機能を付ける
- Next.jsで猫画像ジェネレーターを作ろう
  　Next.jsとは？
  　Next.jsをセットアップする
  　開発サーバーを起動する
  　ページコンポーネントを作る
  　：


用語確認
- Node.js：JavaScriptをサーバーサイドで動かすことを目的に開発されたソフトウェア
- React　：Meta（旧Facebook）が開発したJavaScriptライブラリで、主にユーザーインターフェース（UI）の構築に使用される
- Next.js：ReactをベースにVercel社が開発したオープンソースのJavaScriptフレームワーク
- Vercel ：Next.jsを開発しているVercel社が提供しているフロントエンド向けのクラウドプラットフォーム

今後も利用できる開発環境の作成手順をまとめておきます。
- Node.jsのインストール
  brew install node@24
- シェルの環境変数PATHにNode.jsのパスを追加する
  echo 'export PATH="/opt/homebrew/opt/node@24/bin:$PATH"' >> ~/.zshrc
- Node.jsのバージョン確認
  node -v
- TypeScriptのインストール
  npm install -g typescript
- TypeScriptのバージョン確認
  tsc -v
- Node.jsの実行
  node test.js
- JavaScriptをTypeScriptに変換する
  mv increment.js increment.ts
- TypeScriptの実行
  tsc test.ts
- Reactプロジェクトのひな型作成
　npm create vite@latest like-button -- --template react-swc-ts --no-interactive
- 依存パッケージのインストール
  npm install
- 開発サーバーの起動
  npm run dev


ファイル
.
├── app/
│   ├── favicon.ico
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── node_modules/
├── public/
├── .gitignore
├── eslint.config.mjs
├── .next/
├── next-env.d.ts
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── README.md
└── tsconfig.json



