# Expert Hub PWA

専門家を切り替えながら使うLLMハブ。ショートカットキー対応・BYOK方式。

## ファイル構成

```
expert-hub-pwa/
├── index.html      ← メインアプリ（全機能入り）
├── manifest.json   ← PWA設定
├── sw.js           ← サービスワーカー（オフライン対応）
├── icon-192.png    ← アプリアイコン
├── icon-512.png    ← アプリアイコン（大）
└── README.md       ← このファイル
```

## 公開方法（GitHub Pages）

1. GitHubで新しいリポジトリを作成
2. このフォルダ内のファイルをすべてアップロード
3. Settings → Pages → Branch: main → Save
4. `https://ユーザー名.github.io/リポジトリ名/` で公開完了

## PCでのインストール方法（ユーザー向け）

1. ChromeでURLを開く
2. アドレスバー右のインストールアイコンをクリック
3. 「インストール」→ ホーム画面にアイコンが追加される

## 使い方

1. 初回起動時に Anthropic API キーを設定
2. Ctrl+1〜9 で専門家を直通切り替え
3. 専門家の追加・編集はサイドバーから

## カスタマイズ

専門家の定義はアプリ内から追加・編集できます。
- カスタム指示（システムプロンプト）
- ナレッジ（参照させたい情報）
- ショートカットキー

## 対応LLM（今後拡張予定）

現在: Anthropic Claude (claude-sonnet-4-6)
予定: OpenAI GPT / Google Gemini / ローカル Ollama
