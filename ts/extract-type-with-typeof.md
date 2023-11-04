# Extract Type With _typeof_

通常の式のコンテキストで typeof を使用した場合:

```typescript
console.log(typeof 256); // => number

const arr = [1, 2, 3];
console.log(typeof arr); // => object
```

型のコンテキストで typeof を使用した場合:

```typescript
type NumArrType = typeof arr; // number[] 型
const numArr: NumArrType = [4, 5];
const strArr: NumArrType = ["foo", "bar"]; // compile error
```

このように、型推論で既存の変数から型を抽出することが出来る。

この機能は、コードのスリム化に貢献するため、実際に多用される。

## References

https://oukayuka.booth.pm/items/2368045

## Related Articles
