## How to build on local
1. .env.sampleを.envにコピーする
```
cp .env.example .env
```

2. composerのインストール
```
brew install composer
composer install
```
4. npmを使用しで、node moduleのインストール
```
npm install
```
5. アプルケーションキーを生成
```
php artisan key:generate
```
6. mysqlに接続し、.envで定義したデータベースを作成
```
mysql -u root -h localhost
create database test
```
7. mysqlサーバーを立ち上げる
```
mysql.server start
```
8. マイグレーション＆シード入れる
```
php artisan migrate
php artisan db:seed
```
9.アプリを立ち上げる
```
php artisan serve
```



## 参考
https://laravel-boilerplate.com/7.0/start.html
