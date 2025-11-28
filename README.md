# robosys2025
標準入力から指定された形式で入力された食べ物リストであるテキストを読み込み、カロリーの合計を出力するコマンドです。また、カロリーが日本人男性の一日のカロリー摂取量の基準値である2650kcalを超えると警告が出力されます。
# mkcon
![test](https://github.com/longtaichuanben-max/robosys2025/actions/workflows/test.yml/badge.svg)
## インストール方法
以下のコマンドをターミナルで入力してください。
```
$git clone https://github.com/longtaichuanben-max/robosys2025.git
```
```
$cd robosys2025
```
## 食べ物リストの形式例
"食べ物名 カロリーの数値"のように半角スペース空けて行ごとに情報を記入してください。
例
```
apple 80
banana 84
アジ 144 
```
## 実行例
例：標準入力からテキストファイルを渡すと、指定の形式で入力されたテキストファイルのカロリーの合計値を出力します。例として上記の形式例の内容を渡す。
入力
```
$ cat text.txt | ./mkcon
```
出力
```
$308.0
```
例：カロリーの合計値が日本人男性のカロリー摂取量である2650kcalを超えていた場合は以下のように
出力されます。例として摂取カロリーの合計が3080kcalであった場合を挙げます。
```
$3080.0over!!
```
## 必要なソフトウェア
- Python
  -テスト済みバージョン: 3.7~3.14
- Ubuntu 24.04 LTS
## テスト環境
- Ubuntu 24.04 LTS
## ライセンス
- このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
- © 2025 Ryuta Kawamoto
## 参考文献
- このパッケージは，[ryuichiueda/slides_marp/robosys2025]由来のコード（© 2025 Ryuichi Ueda）
を利用しています。
- このパッケージのディレクトリ構成やテスト方式は，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て参考にしています。
    - [ryuichiueda/slides_marp/robosys2025](https://github.com/ryuichiueda/slides_marp/tree/master/robosys2025)

