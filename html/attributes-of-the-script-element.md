# Attributes Of The Script Element

`defer` 属性を付けることで、**JS ダウンロード**が **HTML パース**と同時並行で行われるようになり、
**HTML パース**の完了後に **JS 実行**がなされる。

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- ... -->
    <script src="app.js" defer></script>
  </head>
  <body>
    <!-- ... -->
  </body>
</html>
```

モジュールスクリプト（`type="module"`）では、defer 属性や Strict mode がデフォルトの挙動である。

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- ... -->
    <script type="module" src="app.js"></script>
  </head>
  <body>
    <!-- ... -->
  </body>
</html>
```

## References

https://takayamato.com/defer_async/

https://qiita.com/irico/items/bd97e1afc737f83b395d

## Related Articles
