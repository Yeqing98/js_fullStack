## q1  js全局执行为我们创建了两个东西：全局对象 和 this关键字
    new 的实现原理：
        1. 创建一个空对象， 构造函数中的this指向这个空对象
        2. 这个新对象被执行[原型]连接
        3. 执行这个构造函数，属性和方法添加到this引用的对象中
        4. 如果构造函数没有返回其他对象，那么就返回这个this， 既创建的新对象， 否则，返回构造函数中返回的对象。

## q2  call bind apply

## q3  深拷贝  浅拷贝
- 浅拷贝：浅拷贝只是拷贝基本类型的数据，如果父对象的属性等于数组或另一个对象，
那么实际上，子对象获得的只是一个内存地址，因此存在父对象被篡改的可能，浅拷
贝只复制指向某个对象的指针，而不复制对象本身，新旧对象还是共享同一块内存。

- 深拷贝：深拷贝就是能够实现真正意义上的数组和对象的拷贝。递归调用"浅拷贝"。
（深拷贝会另外创造一个一模一样的对象，新对象跟原对象不共享内存，修改新对象不
会改到原对象）

## q4  闭包
    闭包的原理：有权限访问其他函数的作用域的函数
    1. 阻止作用域被js垃圾回收
    2. 创建私有变量
    3. 创建块级作用域

## q5  数组去重
    set typeOf includes map reduce
