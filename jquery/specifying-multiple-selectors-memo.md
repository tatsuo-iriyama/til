# 複数のセレクターを指定する方法
- "AND" 条件で指定する場合

```javascript
$('ul.listClass1'); // タグ名="ul" and class="listClass1"
$('ul#listId1');    // タグ名="ul" and id="listId1"
$('[data-element-class="list"][data-element-id="item"]') // data-element-class="list" and data-element-id="item"
```

- "OR" 条件で指定する場合

```javascript
$('ul,.listClass1'); // タグ名="ul" or class="listClass1"
$('ul,#listId1');    // タグ名="ul" or id="listId1"
$('[data-element-class="list"],[data-element-id="item"]') // data-element-class="list" or data-element-id="item"
```