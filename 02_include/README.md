# 02_include

## 外部ファイルをincludeする場合のビルド(g++)
```
g++ main.cpp -I../common -o main
```
`-I`オプションに続けて対象のファイルが存在するパスを指定する。相対パスでも絶対パスでも良い

このオプションで指定したパスが、includeの検索対象に追加される

参考: https://docs.oracle.com/cd/E19957-01/806-4837/Rev.html

### memo

今回インクルードする `sample_header.h` は `cpp_study/common/include/sample_header.h` にある

つまり，上記で指定しているのは相対パス(実行するディレクトリ `cpp_study/02_include` からのパス)

また， `-I` オプションに続けて `/common` までのパスを指定しているので，main.cpp内でヘッダファイルのパスを指定する際は `/common` 以下のみ記述すればよい

<br>

## 外部ファイルをincludeする場合のビルド(make)
`Makefile`の内容を参照のこと。
ビルドのためのコマンドは01と同様

<br>

## 外部ファイルをincludeする場合のビルド(cmake)
`CMakeLists.txt`の内容を参照のこと。
ビルドのためのコマンドは01と同様
