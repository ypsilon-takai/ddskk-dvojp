DDSKK + DvorakJP

DDSKKにDvorakJPのキーバインドを追加しました。
act(azik on skk)の設定をベースに作ったものなので、DvorakJpに沿っていないバインドもあるかもしれません。 日頃これを使っていますが、DvorakJPの機能をフルに使っているわけではないので、自信はありませんです。

# ベースバージョン
DDSKK 15.2 

# 使い方
DDSKKと同様にしてインストールします。

# 設定
以下のような設定を.skkに入れます。

```
;; DvorakJPを使う
(setq skk-use-dvojp t)

;; か行をcで入れるときに辞書の送りがなをちゃんとする。
(setq skk-okuri-char-alist '((\"c\" . \"k\")))

;; 変換候補の選択キーをDvorakに合ったものにする。
;; 変換候補の選択を aoeu.... に変更
(setq skk-henkan-show-candidates-keys '(97 111 101 117 105 100 104 116 110 115 39 44 46 112 103 99 114 108 109 119 118))
```

