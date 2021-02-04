# docker-composeでdjangoの環境を構築する

## 参考
```
https://chibashi.me/development/docker-compose-django-202004/
```
#各種djangoコマンド

##プロジェクトの作成コマンド
```
$ docker-compose run python django-admin.py startproject mysite . 
```
##マイグレーション 
```
$ docekr-compose run python manage.py migrate
```
##スーパーユーザーの作成
```
$ docker-compose run python manage.py createsuperuser
```
## 静的ファイルのコピー
```
$ docker-compose run python manage.py collectstatic
```
#docekr-composeコマンド
## コンテナの起動
###"-d"はバックグラウンドで起動
```
$ docker-compose up -d
```
##コンテナの停止
```
$ docker-compose stop
```
