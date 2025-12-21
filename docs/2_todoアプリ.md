# todo アプリ

todo アプリを作ってもらいましょう。

## setup

### 準備済み

本ワークショップで利用する初期設定がすでにセットアップされています。

```shell
# vite - react のセットアップ
npm create vite@latest todo-app -- --template react-ts

# amplify のセットアップ
npm create amplify@latest -- --template react-vite
```

### サーバの起動

新たにターミナルを立ち上げ、amplify sandbox サーバを起動しておきます。

```shell
cd todo
export AWS_REGION=ap-northeast-1
npx ampx sandbox
```

新たにターミナルを立ち上げ、vite 開発サーバを起動しておきます。

```shell
cd todo
npm run dev
```

## Kiro CLI

### todo アプリ plan

todo アプリを作成するための plan と実行を Kiro CLI にお願いします。

```shell
kiro-cli
> /plan

aws mpcサーバのAmplify ガイド付きワークフローを利用して、ログイン画面付きTodoアプリを設計してください。
現在の状況は以下の通りです。

## プロジェクトセットアップ
* `npm create vite@latest todo-app -- --template react-ts`
* `npm create amplify@latest -- --template react-vite`

## 開発サーバ
* `npm run start` : viteサーバの起動
* `npx ampx sandbox` : amplify sandboxサーバの起動
```

各種質問に回答することで実装を開始してくれます。

### デザイン plan

デザインがシンプルな可能性があるので、そこも修正してもらいましょう。

```shell
kiro-cli
> /plan

/plan Todoアプリのデザインを整えて欲しいです。
```
