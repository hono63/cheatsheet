# Linuxコマンドのチートシート

## ファイルコマンド

`pwd`  
現在のディレクトリの名前を表示する

`ln -s file link`  
fileのシンボリックリンクlinkを作成する

`cat > file`  
標準出力をfileに書き出す

`tail -f file`  
fileが更新されるたびに末尾10行を出力し続ける

## プロセス管理

`ps`  
プロセスを表示

`kill "pid"`  
プロセス番号:"pid"のプロセスを終了

`bg`  
停止中またはバックグラウンドのジョブを表示する; バックグラウンドの停止中ジョブを再会する

`fg`  
最新のジョブをフォアグラウンドに切り替える

## アクセス管理

`chmod "octal" file`  
fileのアクセス権を777とかに変更する。
- 4:(r), 2:(w), 1:(x)
- 所有者、グループ、その他の順

## SSH

`ssh user@host`  
hostへuserとして接続
- `-p`オプションでport指定

`ssh-copy-id user@hose`  
公開鍵を登録

## 検索

`grep "pattern" file`  
file内のpatternを検索
- `-r`オプションでフォルダ内まで再帰的に検索

`locate "pattern"`  
patternを含む全てのファイルを検索

## システム情報

`date`  
日付と時間を表示

`cal`  
今月のカレンダー

`uptime`  
現在のuptimeを表示

`w`  
オンライン状態のユーザ情報を表示

`whoami`  
現在のユーザー名表示

`finger user`  
userの情報を表示

`uname -a`  
カーネル情報を表示

`df`  
ディスク使用状況

`du`  
ディレクトリのディスク使用状況

`whereis app`  
appのバイナリ・manページの場所を確認

`which app`  
デフォルトで使用されるappを確認


## 圧縮解凍

`tar cf file.tar files`  
filesを含むfile.tarという名のtarファイルを作成する

`tar xf file.tar`  
ファイルを展開する
- `v`オプションでverbose表示
- `z`オプションは解凍するとき。拡張子は"tgz"になる？

`gzip file`  
fileを圧縮してfile.gzに  
`gzip -d file.gz`  
解凍

## ネットワーク

`ping host`  
hostへpingし結果を出力

`whois domain`  
domainのwhois情報を取得

`dig domain`  
domainのDNS情報を取得

`dig -x host`  
hostの逆引きをする

`wget -c file`  
一時中断したfileの続きから再開する

## インストール

`./configure`  
`make`  
`make install`  

`dpkg -l pkg.deg`  
パッケージのインストール(Debian)

`rpm -Uvh pkg.rpm`  
パッケージのインストール(RPM)

## ショートカット

`Ctrl+c` 終了  
`Ctrl+z` 中断.fgでフォアグラウンドジョブ、bgでバックグラウンドジョブに切り替える  
`Ctrl+d` or `exit` セッションをログアウト  
`Ctrl+w` 単語を一つ消す  
`Ctrl+u` 行全体を消す  
`Ctrl+r` 最近実行したコマンドを表示  
`!!` 最後に実行したコマンドを繰り返す  

### 参考
- https://www.usptomo.com/TOMONOKAI_CMS/POMPA/20101124/aho.jpg
