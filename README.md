# TeX Live Container Image
TeX Live 環境を提供する コンテナイメージを管理するリポジトリです。

## コンテナイメージ
このリポジトリでは、LaTeX 文書作成用の TeX Live コンテナイメージを提供しています。

通常は、各プロジェクトの `devcontainer.json` から、  
本リポジトリのイメージを利用します。

プロジェクトの作成には、以下のテンプレートリポジトリを使用してください。  
https://github.com/chozetsu-unko/latex-docker-setup

### イメージの取得
```bash
docker pull ghcr.io/chozetsu-unko/texlive-image:latest
```
TeX Live のバージョンを固定したい場合は、タグを指定して利用することもできます。
```bash
docker pull ghcr.io/chozetsu-unko/texlive-image:2026
```

## ディレクトリ構成
```
.
├── .github          # CI/CD
├── Dockerfile       # コンテナイメージ定義
└── texlive.profile  # TeX Live インストール設定
```
