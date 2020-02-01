# isset function memo
- [isset()](https://www.php.net/manual/ja/function.isset.php)に直接NULLを渡すとFatal errorになる
- 値がNULLの変数は問題ない

```php
isset(null) // NG

$hoge = null;
isset($hoge) // OK
```