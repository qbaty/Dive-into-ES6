# Block-scoped

# let 和 const
在ES6里加入了新的关键字 *let* 和 *const*， 这两个新的关键字表示新的定义变量的方式，而他们定义的变量都是基于块级作用域。这是ES6 新引入的概念，*let* 相当于是 *var* 的块级作用域版，而*const* 定义的是块级作用域的常量。*let* 和 *const* 使用起来比 *var* 更加严格一些，在块级作用域中 *let* 和 *const* 定义的变量必须先定义，再使用否则会报错。

```javascript
const JOHN = { name : 'john' };
JOHN.name = 'johnny';//JOHN = { name : johnny }
```

但是const声明过后的变量，他的值是不能改变的，但是如果声明后的变量为对象，数组等引用类型的对象时。他们属性是可以被改变的，不能改变的只是声明后的引用罢了。

```javascript
const JOHN = { name : 'john' };
JOHN = { name : 'johnny' };
console.log(JOHN);//{ name : 'john' }
```
