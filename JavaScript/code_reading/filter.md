```js
function filter(array, predicate) {
  let index = -1
  let resIndex = 0
  const length = array == null ? 0 : array.length
  const result = []
  // ここでは前置インンクリメントだが
  while (++index < length) {
    const value = array[index]
    if (predicate(value, index, array)) {
      // ここでは後置インクリメントを使っているのはなぜ...?
      result[resIndex++] = value
    }
  }
  return result
}
```
