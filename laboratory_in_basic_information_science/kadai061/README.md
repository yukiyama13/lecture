# 課題61 \[アルゴリズムとデータ構造(C)\]

以下のような命令を受け付けて実行することを繰り返す英和辞書プログラムを考える. 命令の区切りは改行で, 1命令中の単語の区切りは空白文字である. 各単語に空白文字は現れないと仮定する.
- `insert <word> <tango>`: `<word>`の翻訳が`<tango>`であるとデータベースに登録する. 既に登録されている場合は上書きする.
- `delete <word>`: `<word>`をデータベースから削除する.
- `search <word>`: `<word>`をデータベースから検索し, その翻訳を表示する. 単語がデータベースに存在しないときには, `(not found)`と表示する.
- `quit`: プログラムを終了する.

内部のデータベースとして二分探索木を使い, 上述の単語帳プログラムをCで作成する. 入力に日本語特有の文字が含まれているが, 特に気にせずにコードを書いても問題はない. また, 正しい入力のみが入力されると仮定する. `string.h`で定義されている関数を用いる. メモリ管理も適切に行う.

## 入出力例
入出力例を`example1`, `example2`に用意している.
