爆速JSONP
=============================================
http://techblog.yahoo.co.jp/programming/bakusoku-jsonp/

## Introduction

JSONPのWeb APIを手軽に使うためのフレームワークです。JavaScriptを書かずに、WebAPIを使ったブログパーツを作ることができます。

## Example

HTMLに以下のようなscriptタグを書いておくと、自動的にdata-XXXで設定されたWeb APIにリクエストし、その結果でHTMLを作り出力します。

```html
<script src="path/to/bakusoku-jsonp-v1.js"
  data-api="http://example.com/some-webapi"
  data-p-param1="parameter">
Hello {{response}}!!
</script>
```

↓ 

```
HTTP/1.1 200 OK
Content-Type: application/json

{"response":"Hello WebAPI!!"}
```

↓ 

```html
<div>
Hello WebAPI!!
</div>
```

## License
MITライセンスにて提供しています。詳しくはLICENSEをご覧ください。