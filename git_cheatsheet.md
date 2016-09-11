# Git のコマンドチートシート

+
|2016/09/11| 新規作成
+

git init
- 新しく初期リポジトリを作成する

git clone [共有リポジトリのURL]
- 共有リポジトリをローカルにクローンして作業ディレクトリを作成

git add [ファイル名]
- 変更したファイルを索引(index)に追加
git add *
- 変更したファイル全てをindexに追加

git commit -m "コミットメッセージ"
- 変更内容がindexからコミットされ、HEADに格納される(共有リポジトリにはまだ反映されていない)
	+ -mは簡単なコミットメッセージを後ろにつける
	+ -mを使わない場合、エディタが立ち上がる
	+ -aオプションをつけると、変更されているファイルが勝手にコミットされる

git status
- 変更内容などを確認できる

git remote add origin [URL]
- 共有リポジトリの情報を追加。先にgithub上で作っておく必要？

git push -u origin master
- 共有リポジトリにローカルの作業内容をプッシュする

[参考URL]
- http://tracpath.com/bootcamp/learning_git_firststep.html
- http://techacademy.jp/magazine/6235
