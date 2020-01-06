# number_format function memo
- PHPの[number_format](https://www.php.net/manual/ja/function.number-format.php)の第一引数に**NULL**を渡すと**0**を返す

```php
<?php
echo number_format(null);
// 0
```