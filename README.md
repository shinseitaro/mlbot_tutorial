mlbotのチュートリアル。
機械学習で仮想通貨の自動売買をするチュートリアルです。

## Jupyterの起動

```bash
docker-compose up -d
```

## Jupyterを開く

http://localhost:8888 をブラウザで開く。

## チュートリアルを開く

Jupyter内でwork/tutorial.ipynbを開く

## チュートリアルの詳しい解説

環境構築方法など

[機械学習で仮想通貨取引をするチュートリアル。python](https://qiita.com/richmanbtc/items/05916384bf9d2b1e2f35)


## 追記

talib さえ構築できればDockerえ動かさなくても大丈夫。
- [TA-Lib](https://mrjbq7.github.io/ta-lib/install.html)

手元の Linux Mint 20.1 では、
`ta-lib-0.4.0-src.tar.gz` をダウンロード後、こんな感じでインストールした

```bash
$ untar and cd
$ ./configure --prefix=/usr
$ make
$ sudo make install

#  make 時に [configure: error: C compiler cannot create executables] エラーが出た場合のみ
$ sudo apt-get install g++ 

# python仮想環境
$ python -m venv .venv
$ source .venv/bin/activate

# pip update
$ pip install -U pip 

# install 
$ pip install -r requirements.txt
``` 

