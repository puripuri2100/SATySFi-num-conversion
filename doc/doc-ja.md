num-conversion version 0.1.1

# 使い方

数字を以下の表記に変換したり、その評価から逆に数字に変換する関数を提供します。

- ローマ数字（大文字と小文字）
- 全角数字
- 漢数字（非位取り記法）

# 提供モジュール

- `NumConversion`

# 提供関数

- `val to-zenkaku : int -> string option`
- `val from-zenkaku : string -> int option`
- `val to-roman-upper : int -> string option`
- `val from-roman-upper : string -> int option`
- `val to-roman-lower : int -> string option`
- `val from-roman-lower : string -> int option`
- `val to-kansujix : int -> string option`
- `val from-kansujix : string -> int option`


# 注意事項

全ての関数において、負の数は扱えません。また、ローマ数字に関しては5000未満という制限があります。

変換ができない文字列や、制限を超える数字が与えられ場合は`None`が返ります。
