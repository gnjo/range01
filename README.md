### range01
```
二つの要素を使い、あらゆる物をゼロからイチの値に納める。
この場合、ハッシュが生成する最大値で最終的にモジュロレート化する必要がある。
ハッシュ装置の最大値以下でモジュロ演算を行わなければならない。
1 hash
2 modulo rate
```
let max=0Xffffff
let anything=...
let hashed=hash(anything)
let range01=hashed%max/max
console.log(range01) //0 - 1
```
