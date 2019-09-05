### range01
~~~~
二つの要素を使い、あらゆる物をゼロからイチの値に納める。
この場合、ハッシュが生成する最大値で最終的にモジュロレンジ化する必要がある。
ハッシュ装置の最大値以下でモジュロ演算を行わなければならない。
1 hash
2 modulo range => x=v%max/max (range x: 0 - 1)

ゼロからイチの範囲に抑える事ができれば、Math.random()を置き換える事も出来る。
この場合、構成要素に因子を持つ値をゼロからイチとして計算できる数値の意味を持つ。
例えば、複数の因子をこの手法でゼロからイチに抑えた場合、あらゆる物を方程式化出来る。

ある構成要素のカタログとは、全てゼロからイチの範囲である。
~~~~
~~~~
let max=0Xffffff
let anything=...
let hashed=hash(anything)
let range01=hashed%max/max
console.log(range01) //0 - 1
~~~~
