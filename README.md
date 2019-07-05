# local_file_provider
ローカルネットワークでファイルを配信する目的で使用するdocker-composeファイルです。
# 使用方法
`docker-compose.yml`と同じ階層に`sync`ディレクトリを作成し、その中に配信したいファイルを配置します。  
起動するには以下のコマンドを実行します。
```
$ docker-compose up -d
```
ファイルをダウンロードするには、`<IPアドレス>:8080/<ファイル名>`にアクセスします。
# 設定
`docker-compose.yml`内で以下の項目の設定を変更できます
* ポート
* 配信するファイルを配置するディレクトリ

# 補足
nginxのイメージを利用しています。

# What's this?
This is a docker-compose file for to provide any files in local network.
# How to use?
Make a directory that is named `sync` into directory that same as `docker-compose.yml`.  
Deploy into it your files to provide.  
To up it, run this command on your terminal.
```
$ docker-compose up -d
```
To download the files, accress to URL `<Your ip address>:8080/<filename>`.
# Settings
You can edit these settings in `docker-compose.yml`.
* Port
* Directory that files to provide deployed into

# Supplement
It use the image of nginx.
