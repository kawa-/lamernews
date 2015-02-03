# Lamernews


[https://github.com/antirez/lamernews (commit a45bbb142d96c22501464ef9e6b3b1f35900c6d2)](https://github.com/antirez/lamernews) からの個人的フォークです。よく出来ていると思うのですが気になるところもちょくちょくあるので、少しずつ改善していきたいと思います。

## 動作方法

#### 1. RedisをPort 10000で立ち上げ

~~~
# Redisのディレクトリに移動
$ ./src/redis-server --port 10000
$ ./src/redis-cli -p 10000
~~~

#### 2. thinで立ち上げ

~~~
$ bundle
$ ./run.sh
~~~

#### 3. [http://localhost:4040/](http://localhost:4040/) にブラウザでアクセス

#### 4. 停止

~~~
$ ./stop.sh
~~~

##### 蛇足

Nginxをリバースプロキシとするには、[Ubuntu、Sinatra、インストール方法、ベンチマーク](http://mitsuakikawamorita.com/blog/?p=1286) を参考にして下さい。

## オリジナル版との違い

- thinで立ち上げられるようにした (2015-02-03)
- README.mdを書いた (2015-02-03)

## ライセンス

オリジナル版に準拠して、two clause BSDとします。