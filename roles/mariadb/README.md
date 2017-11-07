# 初期設定
MariaDBをインストールしたら、以下のコマンドを実行

```
$ mysql_secure_installation
```

また、データベースの文字コードがutf8になっているかを確認する。

```
$ show variables like 'char%';
```

なっていなかったら、設定ファイルを変更しリロードする。


備考
登録されているユーザーの確認

```
$ select user,host,password from mysql.user
```
