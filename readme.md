## 編集を始めるには

### 前提環境
- python 3.6 以上

### 環境構築
以下のコマンドを実行します。

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### プレビュー用サーバの立ち上げ
```
cd pages
mkdocs serve
```

上記コマンドでプレビュー用サーバが立ち上がります。
立ち上がった後は、 `http://localhost:8000/` でプレビューが確認できます。


