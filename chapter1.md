# Quick Start

### array

> no, ndarray , OR numpy.array

ndarray是numpy数据的主要存储方式。

ndarray是齐次多维数组。

1. 它是一张表，表内元素类型相同。
2. 索引是自然数元组。
3. 数组维度叫做轴，轴数叫做阶。

`[1,2,1]`

一阶数组，也就是一个轴，轴长3.

```
[[ 1., 0., 0.],
 [ 0., 1., 2.]]
```

二阶数组，两个轴，第一个轴长度2，第二个轴长度3。

索引从\(0,0\)到\(1,2\)

> 推论1：n+1阶数组的元素是n阶数组，n&gt;0。

`ndarray.ndim`

维数，python称阶。

`ndarray.shape`



_n_

rows and

_m_

columns,

shape

will be

\(n,m\)

. The length of the

shape

tuple is therefore the rank, or number of dimensions,

ndim

.

ndarray.size

the total number of elements of the array. This is equal to the product of the elements of

shape

.

ndarray.dtype

an object describing the type of the elements in the array. One can create or specify dtype’s using standard Python types. Additionally NumPy provides types of its own. numpy.int32, numpy.int16, and numpy.float64 are some examples.

ndarray.itemsize

the size in bytes of each element of the array. For example, an array of elements of type

float64

has

itemsize

8 \(=64/8\), while one of type

complex32

has

itemsize

4 \(=32/8\). It is equivalent to

ndarray.dtype.itemsize

.

ndarray.data

the buffer containing the actual elements of the array. Normally, we won’t need to use this attribute because we will access the elements in an array using indexing facilities.



