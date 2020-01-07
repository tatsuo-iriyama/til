# ヒアドキュメントとNowdocの構文と違い
## ヒアドキュメント構文
```php
$text = 'hello';
echo <<< EOL
input text.
{$text}
EOL;

/*
 * 出力結果
 *
 * input text.
 * hello
 */
```

## Nowdoc構文
```php
$text = 'hello';
echo <<< 'EOL'
input text.
{$text}
EOL;

/*
 * 出力結果
 *
 * input text.
 * {$text}
 */
```

## 構文の違い
- 開始の **EOL** にクォートがついてるかどうか
    - ついてる場合、ヒアドキュメント
    - ついていない場合、Nowdoc

- 変数展開ができるかどうか
    - できるのが、ヒアドキュメント
    - できないのが、Nowdoc
