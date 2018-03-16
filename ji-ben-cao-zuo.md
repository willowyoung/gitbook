# Quick Start

### 基本数学运算

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

随机数使用np.random

```py
x=np.random.random((3,4))
print(x)
print(x.min())
print(x.max())
print(x.sum())
```

```py
[[ 0.99750309  0.50708726  0.14657493  0.23163902]
 [ 0.42269217  0.24059414  0.04362584  0.63432504]
 [ 0.90027412  0.29035431  0.19234124  0.98704591]]
0.043625841934
0.997503092698
5.59405706677
```

### reshape和axis

reshape用来输出不同的形状，axis指定要操作的轴

```py
b = np.arange(12).reshape(3,4)
print(b)
print(b.sum(axis=0))                            
print(b.min(axis=1))                            
print(b.cumsum(axis=0))    
print(b.cumsum(axis=1))   
```

```
[[ 0  1  2  3]
 [ 4  5  6  7]
 [ 8  9 10 11]]
[12 15 18 21]
[0 4 8]
[[ 0  1  2  3]
 [ 4  6  8 10]
 [12 15 18 21]]
[[ 0  1  3  6]
 [ 4  9 15 22]
 [ 8 17 27 38]]
```



