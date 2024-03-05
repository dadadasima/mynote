# This关键字

## 对象创建的过程 和  this的本质

通过new关键字调用构造器时, 构造器返回该类的对象，但这个对象并不是完全由构造器负责创建

```java
String aString = "hello1";
String  bString = new String("hello2");
System.out.println(bString);	//hello2
bString = new String(aString);
System.out.println(bString);	//hello1
```

### 创建一个对象：

1. 分配==对象空间==，并将对象成员变量初始化为0或空
2. 执行属性值的显示初始化
3. 执行构造方法
4. 返回对象的地址给相关的变量

> ##### 对象内存分配的方法有两种：
>
> 	1. 指针碰撞
> 	1. 空闲列表

### this的本质：

“创建好的对象的==地址==”。 由于在构造方法调用前，对象已经创建。

因此，在构造方法中也可以使用this代表“当前对象”

### this的常用方法：

1. 使用this关键字调用重载的构造方法时，避免相同的初始化代码。但只能在构造方法中使用，并且==必须位于第一句==。

2. 在程序中产生二义性之处，应使用this来指明当前对象;

   普通方法中，this总是指向调用该方法的对象。	构造方法中，this总是指向正要初始化的对象。

3. this不能用于static方法中。











