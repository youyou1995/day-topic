#### ["1","2","3"].map(parseInt)
答案：[1,NaN,NaN]
原因：`map`中是一个函数，其中有三个值(currentValue, index, array(原数组)),`parseInt`函数有两个参数，(value, radix(进制默认10))。
所以在运行的时候`parseInt`接受到两个参数，其中parseInt(1, 0) //1
parseInt(2, 1) // NaN
parseInt(3, 2) // NaN