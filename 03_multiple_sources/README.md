# 03_multiple_sources

## ソースファイルが複数ある場合のビルド(g++)
```
g++ main.cpp -I../common lib.cpp -o main
```
ソースファイル名を並べれば良い

### memo

ただし， `main.cpp` では `sample_header.h` をインクルードしているので， `-I` オプションに続けて対象のファイルが存在するパスの指定が必要

`-I` オプションを付けないと，以下のようにエラーが出てしまう
```
fatal error: include/sample_header.h: No such file or directory
```

<br>

## ソースファイルが複数ある場合のビルド(make)
`Makefile`の内容を参照のこと。
ビルドのためのコマンドは01と同様

<br>

## ソースファイルが複数ある場合のビルド(cmake)
`CMakeLists.txt`の内容を参照のこと。
ビルドのためのコマンドは01と同様
