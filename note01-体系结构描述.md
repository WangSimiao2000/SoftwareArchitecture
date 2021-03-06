# 体系结构描述

## 非标准的图形符号

* 特点
  * 语义丰富
  * 语义极不准确
  * 没有形式化基础
* 优点
  * 直观形象
  * 简单易用
* 缺点
  * 由于其术语和表达语义上存在着一些不规范和不精确，从而使得以矩形为基础的传统图形表达方法在不同系统和不同文档之间存在着许多不一致甚至矛盾。

## UML

* 特点
  * 语义极其丰富
  * 语义相对精确
  * 有少量的形式化基础
* 用途
  * 需求分析
  * OO类设计
  * 行为设计和分析
  * 代码自动生成
	
## 模块接口语言MIL

* 特点
  * 语义比较丰富，但局限在实现级别，层次较低
  * 语义精确，有编译器作保证
  * 没有或极少有形式化基础
* 优点
  * 具有严格的语义基础，能够支持对较大的软件单元进行诸如：定义/使用、接口定义和导入/导出等操作。
  * 一般来讲，MIL与实际的实现语言无关，只关注构件的对外表现协议以及构件之间的通讯关系
* 缺点
  * 这些语言处理和描述的软件设计开发层次过于依赖程序设计语言，限制了它们处理和描述比程序设计语言元素更为抽象的高层次软件构架元素的能力。 

## 体系结构描述语言ADL

> 组件+连接件+配置

* 基本元素
  * 组件: 计算或数据存储单元；
  * 连接件: 用于模型化构件间的交互，以及指导这些交互的规则
  * 配置: 描述体系结构的构件与连接件的连接图
* 作用：为软件体系结构的表示、分析、演化、细化、设计等提供支持
  * 定义和描述结构概念
  * 描述一个系统是如何被构件建立起来的
  * 描述如何通过现有的构件生成新的系统
  * 指导从多个不同的设计和实现中挑选最优方案
  * 检验一个设计是否能够满足需求
  * 检测一个需求对系统的隐含影响
  * 根据需求自动化构建系统

# 体系结构的核心概念

## 体系结构的定义

>软件体系结构(SA)：
> * 提供了一个结构、行为和属性的高级抽象
> * 从一个较高的层次来考虑组成系统的构件、构件之间的连接，以及由构件与构件交互形成的拓扑结构
> * 这些要素应该满足一定的限制，遵循一定的设计规则，能够在一定的环境下进行演化。
> * 反映系统开发中具有重要影响的设计决策，便于各种人员的交流，反映多种关注，据此开发的系统能完成系统既定的功能和性能需求。

体系结构 = 构件 + 连接件 + 拓扑结构 + 约束 + 质量

## 核心概念

* 构件
  * 具有某种功能的可复用的软件结构单元
  * 一种可部署单元，它具有规范的接口规约和显式的语境依赖
  * 由构件组装出的软件称为构件化软件
* 接口与服务
  * 一个构件至少有一个接口
  * 一个构件可以提供多重接口
  * 构建内部所实现的功能以服务的形式体现出来，并以接口的向外发布
* 连接
  * 构件间建立和维护行为关联与信息传递的途径
  * 需要:
    * 机制
    * 协议:连接的规约
* 连接件
  * 表示构件之间的交互并实现构件之间的连接
  * 可以看作特殊的构件

# 体系结构模型

## 建立模型的目的：

* 定义
  * 系统、理论或现象的图解性的描述，用来描绘其已知的或推测性质的特性，也用于深入研究它们的特点
* 目的
  * 提供一个理想的论证框架，应用逻辑和数学工具，评估性能，并在多个类似的场景下进行推理。

## SA建模是三个层次

* 图形化模型
* 形式化模型
* 文档化模型

## 4+1视图模型

* 逻辑视图
  * 逻辑视图主要支持系统的功能性需求，即系统提供给最终用户的服务。
  * 在UML中，逻辑视图通常使用以下的图形表达形式
    * 类图
    * 活动图
    * 顺序图
    * 组合结构图
* 进程视图
  * 侧重于系统的运行特性，主要关注一些非功能性的需求。
* 物理视图
  * 主要考虑如何把软件部署到硬件上
  * 它通常要考虑系统性能、规模、可靠性等
  * 在UML中，物理视图通常包括
    * 部署图
    * 包图
    * 交互图
* 开发视图
  * 主要侧重于软件模块的组织和管理。
  * 在UML中，开发视图通常使用构件图
* 用例视图
  * 用例视图用来捕获最终用户所需求的功能性，即“系统应该做什么”
  * 在UML中，用例视图主要包括用例图，然后使用若干个交互图来展示每个用例内部的细节

# 软件体系结构的生命周期

## 软件开发过程

1. 需求分析
2. 建立体系结构
3. 软件设计
4. 实现
5. 测试

## 软件体系结构生命周期

1. 非形式化描述
2. 规范描述
3. 求精及验证
4. 实施
5. 演化和扩展(修改体系结构)
6. 评价和度量(重用体系结构)
7. 终结
