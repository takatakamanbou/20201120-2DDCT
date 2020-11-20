# 20201120-2DDCT

## 2次元DCTの式

TypeII を元にしたもの．

- 変換: $f(x, y) \rightarrow F(u, v)\quad (x, y, u, v = 0, 1, \dots , N-1)$
- 逆変換: $F(u, v) \rightarrow f(x, y)\quad (x, y, u, v = 0, 1, \dots , N-1)$

$$
\begin{aligned}
F(u, v) &= \sqrt{\frac{2}{N}}C(u)C(v) \sum_{x=0}^{N-1}\sum_{y=0}^{N-1} f(x, y) \cos \frac{(2x+1)u\pi}{2N} \cos \frac{(2y+1)v\pi}{2N} \\
f(x, y)&= \sqrt{\frac{2}{N}} \sum_{u=0}^{N-1}\sum_{v=0}^{N-1}C(u)C(v)F(u, v)\cos \frac{(2x+1)u\pi}{2N} \cos \frac{(2y+1)v\pi}{2N}
\end{aligned}
$$

ただし

$$
C(a) = \left\{ \begin{array}{ll} \frac{1}{\sqrt{2}} & (a = 0)\\
1 & {\rm otherwise} \end{array} \right.
$$