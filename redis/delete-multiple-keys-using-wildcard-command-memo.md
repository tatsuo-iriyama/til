# Redisでワイルドカードを使用して複数のkeyを削除するコマンドメモ
```terminal
$ redis-cli keys *key_name* | xargs redis-cli del
```
