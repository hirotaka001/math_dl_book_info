# Notebook補足情報

## 動作確認済み環境情報
2019年3月時点で、Notebookの動作確認は以下の環境で行っています。

### Windows / MAC
Anaconda 2018.12 for Windows(Mac) Installer  
ライブラリ別のバージョンは以下の通りとなっています。

```
python 3.7.1
numpy 1.15.4
pandas 0.23.4
matplotlib 3.0.2
scipy 1.1.0
scikit-learn 0.20.1
Jupyter 4.4.0
```

### Watson Studio
ライブラリ別のバージョンは以下の通りとなっています。

```
python 3.5.5
numpy 1.13.3
pandas 0.21.0
patplotlib 2.1.0
scipy 1.0.0
scikit-learn 0.19.1
Jupyter 4.3.0
```

## 11章のNotebookを動かすための追加手順
　本書p.309に記載したとおり、Anacondaデフォルト環境にKerasのライブラリは導入されていないため11章付属のサンプルコードは稼働しません（Watson Studioでは稼働します）。  
　著者が確認した手順を以下のリンク先にアップしておきましたので参考とされて下さい。

qiita記事  
[Windows/MACのJupyter NotebookからKerasが使えるようにする](https://qiita.com/makaishi2/items/f8512c0c4828ddea51ca)

## Notebookプログラムの制限事項と対応策
2019年3月28日時点で判明しているNotebookプログラムの制限事項と対応策は次の通りです。

|章|プラットフォーム|内容|対策|
|---|---|---|---|
|9|Watson Studio|9章用標準のnotebookが稼働しません。|ch09-multi-classify-studio.ipynbを利用してください。|
|10|Watson Studio|学習にかなりの時間を要します。|学習自体はできるので結果が戻るまで待っていてください。|
|11|Mac|環境によりグラフ描画ができない場合があります。|回避策用のコードを含めたnotbookファイルch11-keras-mac.ipynbを用意しました。必ずこちらを利用して、最初のセルのコードも実行するようにしてください。|

