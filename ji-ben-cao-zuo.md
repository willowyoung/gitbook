# Quick Start

基本数学运算

```py
a = np.array( [20,30,40,50] )
b = np.arange( 4 )
print(a-b)
print(b**2)
print(10*np.sin(a))
print(a<35)
```

```
[20 29 38 47]
[0 1 4 9]
[ 9.12945251 -9.88031624  7.4511316  -2.62374854]
[ True  True False False]
```

会生成相同shape的映射数组，如果改变原本数组，可以用 += \*= 这种。

> 注意\*代表普通乘法，矩阵乘法使用dot函数

```py
A = np.array( [[1,1],[0,1]] )
B = np.array( [[2,0],[3,4]] )
print(A*B)      
print(A.dot(B)) 
A *= 3
print(np.dot(A, B))
```

```
[[2 0]
 [0 4]]
[[5 4]
 [3 4]]
[[15 12]
 [ 9 12]]
```



