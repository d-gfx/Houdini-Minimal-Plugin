# Houdini-Minimal-Plugin 雑なメモ

## ビルド方法
* CMakeLists.txt に Houdini のバージョンを含むパスを直書きしているので適宜自分のインストールしたバージョンに変更する。
* Visual Studio 2017 なら CMakeLists.txt のあるフォルダで右クリックからの「Visual Studio で開く」
* ビルドするとユーザのドキュメントフォルダなどに作られる（例えば C:\Users\ユーザ名\Documents\houdini17.5\dso）

## 確認方法
* Houdini を起動
* メニューから「Windows」→「Hscript Textport」でコマンド date を打てたらオッケー
