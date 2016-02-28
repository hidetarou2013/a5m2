# a5m2

Ubuntu14.04ベースのDocker コンテナイメージ
DBツール A5M2 
日本語化済み
GUIツール
Windows用のツールのため、wineを利用


## 1.git clone

```sh
$ mkdir work && cd $_
$ git clone git@github.com:hidetarou2013/a5m2.git
```

## 2.docker build

```sh
$ cd a5m2
$ time docker build -t hidetarou2013/a5m2 .
```

## 3.docker run

```sh
$ time docker run --name a5m2 -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -d hidetarou2013/a5m2 
```


