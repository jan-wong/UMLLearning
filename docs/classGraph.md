## 类图学习

#### 建模概要

模型是对某种系统的抽象，其目的是在构建这个系统之前先理解它，常见的三种建模设计技术包括类建模、状态建模、交互建模。这三种建模技术从不同的角度描述了系统的不同层面，类模型表现了系统静态化的、结构化的“数据层面”；状态模型表现了系统时序的、行为的“控制层面”；交互模型表现了系统各个对象的“交互层面”

类模型通过描述系统内部类、接口的属性、操作及与其他类、接口的相互关系来捕获系统的静态结构。类模型是三种模型中最重要的，也是最常用的。

#### 类图

常见的类图存在着六大关系：实现、继承(也叫泛化)、依赖、关联、聚合、组合

> 实现(realization)

是指一个类`class`实现了某个`interface`接口，一般语言通过`implements`关键字表明两者的关系，在图形中使用虚线中空箭头表示，由类指向接口。

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/01.png)

> 继承（泛化）(generalization)

是指一个类`class`|`interface`继承了另一个类`class`|`interface`，一般语言通过`extend`关键字来表明两者的关系，在图形中使用实线中空箭头表示，由类|接口指向另一个类|接口。

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/02.png)

> 依赖(dependency)

是指一个类A`class`使用了另一个类B`class`，它们是使用关系，具有临时性、方向性，弱关系性，比如汽车使用汽油。在程序实现上B充当A方法的参数而被临时调用，在图形上使用虚线箭头表示，由类A指向被依赖的类B

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/03.png)

> 关联(association)

是指类之间的一种结构关系，比如房间是由墙组成，它们具有强关系性。在程序实现上一个类充作为另一个类的属性存在。在图形上使用实线箭头表示。

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/04.png)

> 聚合(aggregation)
聚合是关联关系的一种特例。它体现了整体/部分的关系，部分可以属于多个整体，它们各自具有各自的生命周期，比如公司和员工。在图形上使用空心菱形箭头表示。

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/05.png)

> 组合(composition)
组合是关联关系的一种特例。它同样体现了整体/部分的关系，但是部分与整体不可分割，具有共同的生命周期，可谓同生共死，比如人和大脑。在图形上使用实心菱形箭头表示。

![](https://raw.githubusercontent.com/jan-wong/UMLLearning/master/graph/06.png)