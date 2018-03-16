# Quick Start

### np.array

用列表初始化

```py
a = np.array([2,3,4])
```

齐次序列的序列为二阶

```py
b = np.array([(1.5,2,3), (4,5,6)])
```

强制指定类型

```py
c = np.array( [ [1,2], [3,4] ], dtype=complex )
```

```
[2 3 4]
[[ 1.5  2.   3. ]
 [ 4.   5.   6. ]]
[[ 1.+0.j  2.+0.j]
 [ 3.+0.j  4.+0.j]]
```

归零，以shape为输入

```py
np.zeros( (3,4) )
```

归一，以shape为输入

```py
np.ones( (2,3,4), dtype=np.int16 )
```

不初始化，随机内存数据

```py
np.empty( (2,3) )
```

```
[[ 0.  0.  0.  0.]
 [ 0.  0.  0.  0.]
 [ 0.  0.  0.  0.]]
[[[1 1 1 1]
  [1 1 1 1]
  [1 1 1 1]]

 [[1 1 1 1]
  [1 1 1 1]
  [1 1 1 1]]]
[[  1.39069238e-309   1.39069238e-309   1.39069238e-309]
 [  1.39069238e-309   1.39069238e-309   1.39069238e-309]]
```

### numpy.set\_printoptions

打印参数，详看[https://docs.scipy.org/doc/numpy/reference/generated/numpy.set\_printoptions.html](https://docs.scipy.org/doc/numpy/reference/generated/numpy.set_printoptions.html)

