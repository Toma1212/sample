## 起動方法
```
$ docker-compose build #初回のみ
$ docker-compose up -d
$ docker-compose exec app bash
ワークスペース
# cd laravel
# php artisan migration
```

## jsファイルの変更時
```
$ docker-compose exec app bash
ワークスペース
#　cd laravel
#  npm run dev (or) npm run watch
```
