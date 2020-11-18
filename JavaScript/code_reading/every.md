```js
function every(array, predicate) {
  let index = -1
  const length = array == null ? 0 : array.length

  while (++index < length) {
    if (!predicate(array[index], index, array)) {
      // 引数のpredicate関数の結果がfalseならfalseを返す
      // 引数の配列の要素に一つでもfalseになるものがあればwhileを抜けている
      return false
    }
  }
  return true
}
```

predicate: 引数arrayを回す度に実行される関数。
++index: 前置インクリメント演算子は、インクリメント後の値を返す。
