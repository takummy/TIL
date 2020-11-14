###### よくお世話になっているので中身を見てみる。

```js
function isNil(value) {
  return value == null
}
```
  
等価演算子で引数valueとnullを比較した結果を返している。  
なので、nullかundefinedの場合にtrueになる。  
めちゃくちゃ単純なことをしてるだけだった…。  
  
ちなみに**isNull**はこんな感じ。  

```js
function isNull(value) {
  return value === null
}
```
  
厳密等価演算子で引数valueとnullを比較した結果を返している.  
なるほどね。。
