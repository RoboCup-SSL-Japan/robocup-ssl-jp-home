# 開発者向け情報

## 前提条件

開発環境は以下の環境で動作確認しています。

- Ubuntu 18.04 LTS on WSL2


## 環境構築
1. 開発を行う環境へ次のアプリケーションをインストールします。
    - python 3.6 以上
    - Git

    Linux(Debian系)の場合は以下のコマンドを実行してください
    ```
    sudo apt update
    sudo apt install python-3.8 git
    ```

2. 本リポジトリをCloneします。  

    Linuxの場合は以下のコマンドを実行してください
    ```
    git clone https://github.com/RoboCup-SSL-Japan/robocup-ssl-jp-home.git
    cd robocup-ssl-jp-home
    ```

2. Pythonの仮想環境の有効化およびパッケージインストールを行います。

    Linuxの場合は以下のコマンドを実行してください

    ```
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

## 編集

本HPは [MkDocs](https://www.mkdocs.org/) および [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) を用いて構成されています。

HPのコンテンツは `pages/docs` 以下のマークダウンファイルに記述されています。  
コンテンツを追加するには `pages/docs` 以下にマークダウンファイルを配置した上で `pages/mkdocs.yml` の `nav` 以下にマークダウンファイルのパスを追加してください。

その他詳細な使用方法は、 MkDocs または Materialfor MkDocs のドキュメントを参照してください。

## プレビュー

ローカル環境でHPのプレビューをするには以下のコマンドを実行して、プレビュー用サーバを立ち上げてください。

```
cd pages
mkdocs serve
```

立ち上がった後は、 `http://localhost:8000/` でプレビューが確認できます。

## 実際のHPへの反映

Github上の master ブランチの内容が自動的にHPに反映されるようになっています。  
PRが管理者によって承認され master ブランチにマージされると、実際のHPへの反映が行われます。
