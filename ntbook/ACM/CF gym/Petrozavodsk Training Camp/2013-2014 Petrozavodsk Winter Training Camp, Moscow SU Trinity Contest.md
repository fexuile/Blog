# 2013-2014 Petrozavodsk Winter Training Camp, Moscow SU Trinity Contest

## Problem A. MEX-Query


```cpp

```

## Problem D. Short Enough Task


## Problem F. Just Another Sequence Problem
不妨设$f_{i,j}$表示当前到了第$i$位，这次分割出来的是$[j,i]$这一段区间，那么很明显可以$\Theta(n^3)$的进行$dp$。

考虑对这个式子化简：  
```mathjax
$$
\begin{aligned}
f_{i,j}&=\max_{k=1}^{j-1}f_{k,j-1}+(s_i-s_{j-1})*(s_{j-1}-s_{k-1})\\
&=s_i\times s_{j-1}-s_{j-1}^2+\max_{k=1}^{j-1}\{f_{k,j-1}-(s_i-s_{j-1})\times s_{k-1}\}
\end{aligned}
$$
```  

这