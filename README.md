# Morse-Code-Simple-Converter
モールス符号の相互変換を行う簡易的なコマンドラインツール

## 使い方

morse [-d] ...

-d,  復号


|モールス符号|表記|
|:-:|:-:|
|トン(dots)   |.|
|ツー(dashes) |-|
|区切り       |半角スペース |

アルファベットの大文字・小文字は不問

テスト用なので別の文字を使いたいときは tr コマンドで

## 例

`morse SOS`
-> `... --- ...`

`morse -d '... --- ...'`
-> `SOS`

`morse 'morsecode' | morse -d`
-> `MORSECODE`
