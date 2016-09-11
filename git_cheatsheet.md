# Git のコマンドチートシート

`git init`
- 新しく初期リポジトリを作成する

`git clone [共有リポジトリのURL]`
- 共有リポジトリをローカルにクローンして作業ディレクトリを作成

`git add [ファイル名]`
- 変更したファイル/ディレクトリを索引(index)に追加  

`git add *`
- 変更したファイル全てをindexに追加

`git commit -m "コミットメッセージ"`
- 変更内容がindexからコミットされ、HEADに格納される(共有リポジトリにはまだ反映されていない)
	+ `-m`は簡単なコミットメッセージを後ろにつける
	+ `-m`を使わない場合、エディタが立ち上がる
	+ `-a`オプションをつけると、変更されているファイルが勝手にaddされてコミットされる

`git status`
- 変更内容などを確認できる

`git remote`
- リモートリポジトリの名称一覧を表示  

`git remote -v`
- リモートリポジトリの詳細一覧を表示  

`git remote add origin [URL]`
- 共有リポジトリの情報を追加。先にgithub上で作っておく必要？  

`git remote rm [name]`
- リモートリポジトリを削除

`git push -u origin master`
- 共有リポジトリにローカルの作業内容をプッシュする

`git branch [branch-name]`
- ブランチの作成

`git branch`
- ブランチの一覧表示

`git branch -d [branch-name]`
- 指定したブランチを削除

`git checkout [branch-name]`
- ローカルリポジトリのブランチを切り替える

`git log`
- ローカルリポジトリのコミット履歴を閲覧
	+ `-n`オプションで履歴の表示数を指定

`git grep [search-word]`
- リポジトリのファイルの内容から検索

#### 参考URL
- http://tracpath.com/bootcamp/learning_git_firststep.html
- http://techacademy.jp/magazine/6235
