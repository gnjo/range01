### range01
~~~~
二つの要素を使い、あらゆる物をゼロからイチの値に納める。
この場合、ハッシュが生成する最大値で最終的にモジュロレート化する必要がある。
ハッシュ装置の最大値以下でモジュロ演算を行わなければならない。
1 hash
2 modulo rate

ゼロからイチの範囲に抑える事ができれば、Math.random()を置き換える事が出来る。
この場合、構成要素に因子を持つ値をゼロからイチとして計算できる数値の意味を持つ。
~~~~
~~~~
let max=0Xffffff
let anything=...
let hashed=hash(anything)
let range01=hashed%max/max
console.log(range01) //0 - 1
~~~~
