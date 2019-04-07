我是第一次完整写C#的程序，由于C#是在C++基础上改进的语言，故而我自认为还是可以圆满完成这个任务的。


- [准备](#准备)
- [题目](#题目)
- [要求](#要求)
    - [设计模式](#设计模式)
        - [模板方法模式](#模板方法模式)
        - [代理模式](#代理模式)
    - [UML图示](#uml图示)
        - [作图工具](#作图工具)
        - [类图的设计](#类图的设计)
        - [时序图](#时序图)
        

## 准备

在做题之前，首先安装好IDE工具[Visual Studio](https://visualstudio.microsoft.com/zh-hans/vs/)。

## 题目

用C#实现一个小型连锁超市的**库存管理**，连锁超市在全国可能有多个仓库，可以查询指定仓库的商品库存情况，实现以下功能：

- 商品信息管理（增删改查）
> 商品编号+ 名称+类型+单价+计量单位+数量

- 货架信息管理（增删改查）
> 货架编号+总层数

- 仓库信息管理（增删改查）
> 仓库编号+地址

- 商品出库/入库管理
> 本质是对不同对象“增删改查”操作的综合运用

- 查询库存数量前三名的商品              
- 统计指定仓库所有商品总价值       
- 退出系统

- 录入及修改后的数据需保存到本地文件或数据库

## 要求

需要注意的要求有两个：

- 采用一到两种**设计模式** 
- UML画系统的**类图**和入库的**时序图**

### 设计模式

非科班的我对[设计模式](http://www.runoob.com/design-pattern/design-pattern-tutorial.html)的理解，只停留在走马观花地看了一遍《设计模式之禅》、知道设计模式有23种之多的程度上。

#### 模板方法模式

看看这个项目，使用到**模板方法模式**是肯定的，因为毕竟仅仅是使用类的继承机制，就符合模板方法模式的定义：

> Template Method Pattern. Define the skeleton of an algorithm in an operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure.

#### 代理模式

此外，使用**代理模式**应该也不容置疑。它是一个使用率非常高的模式，提供访问控制。定义如下

> Proxy Pattern. Provide a surrogate or placeholder for another object to control access to it.

根据《设计模式之禅》，代理模式有3个角色：

- Subject抽象主题角色
- RealSubject具体主题角色
- Proxy代理主题角色

Proxy负责对真实角色的应用，把所有Subject定义的方法**限制委托**给RealSubject角色实现，并且在RealSubject处理过程的前后做预处理和善后处理。

### UML图示

软件工程是系统性极强的，**统一建模语言(UML)**可以帮助软件开发者们梳理系统的各种逻辑。

非科班的我看了《构建之法》和《UML2与Rose建模从入门到精通》，大致知道怎么回事。

#### 作图工具

- 听说Rose是主流的画UML图的工具，可是网上破解版都是2007。
- Visio是office系列的，周围人用的多些。
- 但我还是喜欢很简洁的在线作图网站[ProcessOn](https://www.processon.com/)，因为在哪都可以用。

#### 类图的设计

待填坑

#### 时序图

待填坑
