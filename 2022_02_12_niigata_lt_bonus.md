---
marp: true
theme: gaia
backgroundColor: #fffafa
footer: "2022-02-12 北海道未完×デルタ新潟合同LT会 おまけ https://twitter.com/manattan_me"
paginate: true
---

# macbook の環境を git 管理しました

### 北海道大学工学部　もぎたかのり

---

### 前提

- Time Machine は、新しい PC になった時意味ないですよね？（外付けにすれば大丈夫そう？）
- そもそも local に写真とかメールとか入れてないからそんなことしなくていいよね？（クラウドに保存することが多いよね？）

---

# こんなのを作りました

https://github.com/manattan/environment

### クリーンインストールしたり mac を新しく買う時、元の設定を引き継ぎたい事項ってなんだろう？

- VScode の設定 / 拡張機能
- ターミナルの設定（.bash_profile, .zshrc ...）
- brew install したやつ

---

### 使い方

- `make setup`
  - homebrew を入れる(必要な ruby はもともと入っている！)
- `make package/install`
  - Brewfile を読み込んで、brew install してくれる！
- `./vscode/install.sh`
  - 拡張機能をインストールしてくれる！

---

### よかったこと

- 不要なファイルはいらないよね
  - 一時的に使いたいソフトを brew でインストールしたら無駄に容量食っちゃうけど、リポジトリのファイルを更新しなかったら次回以降インストールされないよね！
  - 必要なものだけを`Brewfile`に入れればいい！
- 新しい PC の設定めっちゃ便利！

---

まとめ

- Time Machine もいいですが、mac の中だけに保存するものがほぼなければこれで十分！

- なんでもクラウドに入れる癖がつきました。
