# Morse-Code-Simple-Converter
モールス符号の相互変換を行う簡易的なコマンドラインツール
自分用の想定で作ったのであまり当てにしない方が良いです

## 使用方法

morse [-h][-d] [infile]

  -h, --help    ヘルプ
  -d, --decode  復号

|モールス符号|表記|
|:-:|:-:|
|トン(dots)   |.|
|ツー(dashes) |-|
|区切り       |半角スペース |



別の文字を使いたいときは tr コマンドで

### 利用可能な文字

ABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890,.?/-()

アルファベットの大文字・小文字は不問

## 例

`echo SOS | morse`
-> `... --- ...`

`echo '... --- ...' | morse -d`
-> `SOS`
