# 学习通作业知识点汇总

#### 体系结构发展过程经历的四个阶段

1. 无体系结构设计阶段
2. 萌芽阶段
3. 初级阶段
4. 高级阶段

#### 软件体系结构的含义及组成

1. 软件体系结构为软件系统提供了一个结构、属性和行为的高级抽象。它不仅指定了系统的组织结构和拓扑结构，并且显示了系统需求和构成系统的元素之间的对应关系，提供了一些设计决策的基本原理。
2. 体系结构由构件、连接件、约束组成

#### 软件重用的含义,意义,可重用元素

1. 含义:软件重用是指在多次不同的软件开发过程中重复使用相同或相近软件元素的过程。
2. 意义:软件重用是软件产业工业化、工程化的重要手段。软件重用对提高生产率，降低开发成本，缩短开发周期，改善软件质量以及提高灵活性和标准化程度大有帮助。
3. 种类:可重用的元素包括程序代码、测试用例、设计文档、需求分析文档甚至领域知识。可重用的元素越大，我们就说重用的粒度越大。

#### 常用的构件实现模型及其意义

1. 实现模型：
   1. CORBA
   2. EJB
   3. COM / DCOM / COM+
2. 意义：这些模型通常都定义了构件的实现方式、接口定义、访问方法等。符合这些标准的任何构件都有很高的重用能力。

#### 体系结构的描述方式

1. 非标准的图形符号
2. UML
3. 模块接口语义MIL
4. 软件体系结构的描述语言ADL

#### 体系结构的核心模型的最基本的元素

1. 构件
2. 连接件
3. 约束

#### "4+1"视图

* 4:
  * 逻辑视图--最终用户:功能需求
    * 包图、类图、对象图（静态部分）或序列图、协作图、状态图和活动图
  * 进程视图--系统集成人员:性能可扩充性,吞吐量等
    * 包图、类图、对象图（静态部分）或序列图、协作图（动态部分）
  * 物理视图--系统工程人员:系统拓扑,安装,通信
    * 部署图和构件图
  * 开发视图--编程人员:软件管理
    * 包图、类图、构件图
* 1:
  * 用例/场景视图
    * 例图、活动图、顺序图

#### 建立软件体系结构模型的作用

1. 用户、软件架构师、开发者等各方人员之间的交流
2. 分析、验证SA设计的优劣
3. 指导软件开发组进行软件开发
4. 为日后的软件维护提供基本文档

#### SA建模的三个层次

1. 图形化模型： 
2. 形式化模型：
3. 文档化模型：

#### 软件体系结构生命周期的主要阶段

1. 非形式化描述
2. 规范描述
3. 求精及验证
4. 实施
5. 演化和扩展(修改体系结构)
6. 评价和度量(重用体系结构)
7. 终结

#### 体系结构风格

* 数据流风格
   * 批处理
   * 管道-过滤器
   * 过程控制
* 调用/返回风格
  * 主程序与子程序
  * 面向对象风格
  * 层次结构
* 独立构件风格
  * 进程通信
  * 事件系统
* 虚拟机风格
  * 解释器
  * 基于规则的系统
* 仓库风格
  * 数据库系统
  * 超文本系统
  * 黑板系统

#### 管道过滤器风格的基本构成元素

* 构件: 过滤器Filter
* 连接件Connectors: 管道
* 拓朴结构Topology: 连接器定义了数据流图,形成拓扑结构

#### 黑板系统的组成

* 知识源
* 黑板数据结构
* 控制器

#### 松散分层的含义及优缺点

1. 含义: 允许构件与位于它下面的任意层中的组件进行交互的分层模式称为松散分层
2. 优点：松散方法可以改善效率，因为系统不必将简单调用从一层转发到下一层
3. 缺点：松散方法在层之间不提供相同的隔离级别，这使得在不影响较高层的情况下换出较低层变得更困难

#### 隐式调用系统的优缺点

* 优点
  * 为软件重用提供了强大的支持
  * 为改进系统带来了方便。
* 缺点
  * 构件放弃了对系统计算的控制
  * 数据交换的问题
  * 既然过程的语义必须依赖于被触发事件的上下文约束，关于正确性的推理就存在问题

#### MVC风格的含义

* 模型: 商务逻辑
* 视图: 外观呈现
* 控制器: 请求处理

#### 常用的软件体系结构评估方法

1. 基于调查问卷或检查表的评估方式
2. 基于场景的评估方式
3. 基于度量的评估方式

#### 软件质量属性

1. 性能
2. 可靠性
   1. 容错
   2. 健壮性
3. 可用性
4. 安全性
5. 可修改性
   1. 可维护性
   2. 可扩展性
   3. 结构重组
   4. 可移植性
6. 功能性
7. 可变性
8. 可集成性
9.  互操作性