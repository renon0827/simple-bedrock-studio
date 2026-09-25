# Simple Bedrock Studio

Amazon Bedrock の API キーだけで、スマホのブラウザから画像生成とチャットを試せる 1 ファイルの Web アプリです。

**公開ページ:** https://renon0827.github.io/simple-bedrock-studio/

## 使い方

1. AWS コンソールで Bedrock の API キーを発行する（短期キー推奨）
2. ページを開いて「設定」に API キーを入力する
3. 「画像生成」または「チャット」タブで試す

## 対応モデル

| 種類 | モデル | 主なリージョン |
| --- | --- | --- |
| 画像 | Amazon Nova Canvas | us-east-1 / ap-northeast-1 / eu-west-1 |
| 画像 | Stable Image Core / Ultra, SD3.5 Large | us-west-2 |
| チャット | Converse API 対応モデル（Nova, Claude など。モデル ID は自由入力） | 各リージョン |

## セキュリティ

- サーバーはありません。ブラウザから `bedrock-runtime.<region>.amazonaws.com` へ直接リクエストします。
- API キーは「この端末に保存する」をオンにした場合のみ、そのブラウザの localStorage に保存されます。
- 共用端末では保存しないでください。長期キーを使う場合は有効期限を短めにしてください。
- 利用料金は API キーを発行した AWS アカウントに通常どおり課金されます。
