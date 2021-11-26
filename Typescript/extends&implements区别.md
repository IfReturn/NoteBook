# extends & implements 区别
- extends 该类从父类获取所有的属性和方法，不需要实现
- implements 该类从父类获取属性和方法的定义，但是需要实现出来

```
class Person {
  name: string;
  age: number;
}
class Child extends Person{
  // 无需实现定义，全部继承过来了
}
class Man implements Person{
  // 需要实现定义，这里相当于要求 Man 的定义要和 Person 一致，需要自己去定义
  name: string;
  age: number;
}
```
