1. 图片边框都用代码写，图片自带的边框又虚化

```
// JSON.stringify(对象，过滤器，json字符串缩进选项)会将对象转化为JSON字符串格式，对象的函数和原型上的成员会被忽略，职位undefined的属性也会被忽略
    // 过滤器如果是数组则是要包含过滤的字符串属性的数组
    // 过滤器如果是函数，则会将对象的每项进行递归过滤，直到传入过滤器的是键值对，如果该属性返回值是undefined，则该属性不会序列化
    // 注意事项
    // 1. 转换的值中有NaN或者Infinity，则会将值序列化为null
    // 2. 被转换值中有undefined，函数和Symbol
    //    - 数组：在序列化过程中这些转为null
    //    - 对象：在序列化过程中这些被忽略
    // 3. 对象的属性值通过某种间接的方式指回该对象本身,那么序列化会报错
    // 4. 不可枚举的属性值序列化也会被忽略
```

