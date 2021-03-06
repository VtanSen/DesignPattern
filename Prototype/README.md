## 原型模式

### 概述
用原型实例制定创建对象的类型，并通过拷贝这些原型创建新的对象。原型模式会要求对象实现一个可以“克隆”自身的接口，这样就可以通过拷贝或者是克隆一个实例对象本身来创建一个新的实例。如果把这个方法定义在接口上，看起来就像是通过接口来创建了新的接口对象。通过原型实例创建新的对象，不再需要关心这个实例本身的类型，也不关心它的具体实现，只要它实现了克隆自身的方法，就可以通过这个方法来获取新的对象，而无须再去通过new来创建。

### 结构图
![原型模式结构图](http://7u2eqw.com1.z0.glb.clouddn.com/原型模式结构图.png)

### 实现
使用文章接口来实现原型模式。并使用深度克隆，即除了克隆按值传递的数据，还负责克隆引用类型的数据。

### 总结与分析
原型模式的本质是克隆生成对象。克隆是手段，目的是生成新的对象实例。原型模式可以用来解决“只知接口而不知实现的问题”。如果需要实例化的类是在运行时刻动态指定时，可以使用原型模式，通过原型来得到需要的实例。
