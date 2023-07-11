####　第三回課題提出

1. APサーバーについて調べてみましょう
* APサーバーの名前とバージョン
~~~~
$ bin/rails s
....
Puma version: 5.6.5 (ruby 3.1.2-p20) ("Birdie's Version")
~~~~
* APサーバーを終了させた場合、引き続きアクセスできますか？
> できません。
![APserverdown](https://i.ibb.co/RY3Lj2y/APserverdown.png)
* 結果確認して、またAPサーバーを起動してください。
![APserveron](https://i.ibb.co/cxN3vCb/APserveron.png)
2. DBサーバーについて調べてみましょう
* DBサーバーの名前とバージョン
~~~~
 $ mysql --version
mysql  Ver 8.0.33 for Linux on x86_64 (MySQL Community Server - GPL)
~~~~
* DBサーバーを終了させた場合、引き続きアクセスできますか？
> できません。
![DBserverdown](https://i.ibb.co/3pkcc31/DBserverdown.png)
3. Raiseの構成管理ツールの名前は何でしたか？確認してみてください。
~~~~
$ bundler --version
Bundler version 2.3.14
~~~~
4. 今日の課題から学んだこと：

> APザーバーとDBサーバーどちらか一つダウンした場合、サービスにサクセスできなくなります。

> 外部ライブラリ:便利機能を集めて構成させたもの。例：Ruby on Rails
階層関係：機能/モジュールファイル＞パッケージ(gem)＞外部ライブラリ(Rails)

> 複雑なアプリケーションを作ろうとする場合、gemのバージョンやgemを動かせるためのgemが入っているか管理するのが大変なので、
構成管理ツール(Bundler)が必要になります。

> MySQLサーバーの停止・再起動コマンド：
起動:  sudo service mysqld start
状態確認:  sudo service mysqld status
停止: sudo service mysqld stop
再起動: sudo service mysqld restart