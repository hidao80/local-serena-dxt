# Local Serena DXT

![Claude Badge](https://img.shields.io/badge/Claude_Extension-D97757?logo=claude&logoColor=fff&style=flat)
[![License][License-Badge]][License]

## 概要

ローカルにある任意のプロジェクトでSerena MCPを起動し、ClaudeデスクトップアプリからアクセスできるようにするClaudeデスクトップ拡張機能（DXT）です。

## インストール方法

1. Claudeデスクトップアプリを起動します。
2. [設定]->[拡張機能]画面へ移動し、[詳細設定]ボタンをクリックします。[詳細設定]画面へ移動します。
3. [拡張機能をインストール]ボタンをクリックします。ファイル選択ダイアログが開くので、[local-serena.dxt]を選択して[プレビュー]ボタンをクリックします。
4. プレビューダイアログが開くので[インストール]ボタンをクリックします。
5. 設定ダイアログが開くので対象とするプロジェクトとポート番号を指定します。
6. 設定ダイアログが閉じるので、プレビューダイアログで[無効]になっているトグルスイッチをクリックし、[有効[にします。このタイミングでSerena MCPが起動します。
7. プレビューダイアログを閉じます。

## 使い方

Claudeデスクトップアプリを起動し、Local Serana DXTを有効にするとSerenaが起動します。

この状態でClaudeデスクトップアプリからチャットで「Serenaでプロジェクトの〇〇を教えて」などの
プロンプトを入力すると、ClaudeデスクトップアプリがSerenaを操作して情報を返します。 

必要に応じてファイルの読み取りやSerenaのメモリーファイルへの書き込みを行います。

## ビルド方法

<details>
<summary>手順</summary>

```sh
# uvとnpmをインストールします。
winget install astral-sh.uv OpenJS.NodeJS.LTS

# このリポジトリをクローンします。
git clone https://github.com/hidao80/local-serena-dxt

# 今cloneしたlocal-serenaディレクトリに移動します。
cd local-serena-dxt

# ビルドスクリプトを実行します。
npm run package
``` 

</details>

## ディレクトリ構成

<details>
<summary>ディレクトリツリー</summary>

```
serena-dxt/
├── .gitignore
├── README.md
├── README_ja.md  ← このファイル
├── package.json
└── src/
    ├── .dxtignore
    ├── icon.png
    └── manifest.json
```

<description>
</details>

## ライセンス

MIT