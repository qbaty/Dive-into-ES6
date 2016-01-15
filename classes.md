# Classes
ES 6 引入了Class 类的概念，先来看看什么样是一个Class 吧：

```javascript
class Person extends Animal {
  constructor(name) {
    super()
    this.name = name;
  }
  say(words) {
    console.log(words);
  }
}
```
