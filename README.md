# LangChainLambda
### 2023/11末に実施する発表のためのリポジトリです。

## ゴール
#### ※2023/11/3時点の想定
参加メンバーでチャットボット経由のLLM実行を「自ら手を動かして」実装することで、
- GPT 3.5できること/できないことの知見を得る
- 開発環境/実行環境がサーバレスである(やや)モダンな開発を体験し、その知見を得る

上記から今後のやってみたいこと、できそうなことを言語化し、発表の材料とする

# 構成
- SlackからWebhook経由でLambdaにhttpsリクエストを飛ばし、返答を返す
- Lambda上ではPython/LangChainの実装で、OpenAIのWebAPIを実行し、gpt-3.5 turboからの返答を返す


# やること
- Cloud9環境の準備 - [x]
- Slackチャンネルの作成 - [x]  
- Slackアプリの作成 - [x]  
- SlackOAuthトークンの取得 - [x]
- OpenAI keyの設定 - [x] 
- ソケットモードの有効化 - [x]  
- アプリケーションの作成 - [x]  
- イベント設定 - [x]  
- Momento Chacheの設定  - [ ]  
- Lazyリスナーの設定  - [ ]  
- AWS Lambdaへのデプロイ - [ ]  
- AWS LambdaLayerの作成 - [ ] 

# 開発環境構築手順
https://qiita.com/hamanuman/items/4736eecb2134b2b86c90

# SlackBot設定手順
https://qiita.com/hamanuman/private/4dca7eecc819355e13bf

# MomentoChacheキー取得方法
https://qiita.com/hamanuman/private/2853f6d0cd2d1125afdc

# 参考資料
「ChatGPT/LangChainによるチャットシステム構築［実践］入門」 第7章
https://www.amazon.co.jp/ChatGPT-LangChain%E3%81%AB%E3%82%88%E3%82%8B%E3%83%81%E3%83%A3%E3%83%83%E3%83%88%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E6%A7%8B%E7%AF%89%EF%BC%BB%E5%AE%9F%E8%B7%B5%EF%BC%BD%E5%85%A5%E9%96%80-%E5%90%89%E7%94%B0-%E7%9C%9F%E5%90%BE/dp/4297138395/ref=sr_1_1