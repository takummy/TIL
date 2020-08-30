## Currying

普通の関数
```js
const multi = (n, m) => n * m;
multi(2, 4); // 8
```

カリー化すると
```js
const curriedMulti = n => m => n * m;
curriedMulti(2)(4); // 8
```

先に1つ目の引数だけ渡しておくことができる
```js
 const double = curriedMulti(2);
 double(4); // 8
 ```