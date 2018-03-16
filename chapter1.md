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

n行m列，shape就是\(n,m\)

shape元组的长度就是维数，ndim

`ndarray.size`

元素总数量，shape元组所有元素的乘积。

`ndarray.dtype`

数组元素类型，包括python标准类型和numpy的基本类型。

`ndarray.itemsize`

元素的大小，单位bytes，float64就是\(64/8\)=8。object的itemsize是8。

等价ndarray.dtype.itemsize

`ndarray.data`

the buffer containing the actual elements of the array. Normally, we won’t need to use this attribute because we will access the elements in an array using indexing facilities.

