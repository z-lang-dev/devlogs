# Z语言炼成记

## 介绍

Z语言是一门面向个人的、专注于学习和探索的编程语言。

Z语言着力于编译器相关知识的学习和分享，注重内容的广度，深度上则是由浅及深。

Z语言的实现放在<https://gitee.com/z-lang/zc>工程里。

《Z语言炼成记》这本书用来记录我在设计和开发Z语言过程中产生的思考和经历，希望能够让大家更有临场感地去了解Z语言。

我打算采用日志的形式来记录，每做一部分代码，就更新一节。
但我并不能保证每天都有更新，毕竟编译器这种非常繁杂的工作，不可能每天都有值得分享的产出。

话题的形式确定为“一天以内能解决的问题”，如果不能，就分成好几篇。

关于Z语言的更多介绍，可以参看：[Z语言是什么](./Z语言是什么.md) 一节。

## 目录

#### 引言

- [Z语言是什么](./Z语言是什么.md)。

#### 第一章：基本框架

1. [最简单的Z程序](./第一章/最简单的Z程序.md)。
1. [最简单的编译器Linux版](./第一章/最简单的编译器.md)。
1. [最简单的编译器Windows版](./第一章/最简单的编译器Windows版.md)。
1. [最简单的转译器](./第一章/最简单的转译器.md)。
1. [最简单的交互器](./第一章/REPL.md)。
1. [组织代码结构](./第一章/组织代码结构.md)。
1. [自动测试](./第一章/自动测试.md)。

#### 第二章：算数运算

1. [整数](./第二章/整数.md)。
1. [词法分析](./第二章/词法分析.md)。
1. [加法](./第二章/加法.md)
1. [四则运算](./第二章/四则运算.md)
1. [优先级和括号](./第二章/优先级和括号.md)

#### 附录

- [参考资料](./参考资料.md)。

## 短期规划

2023年11月目标：

- 书：写完前四章。第五章写一半，实现基本的面向对象：类型、方法和简单继承。
- Z语言：实现v0.1版，一个可用的玩具语言，同时支持动态解释、静态编译，还能够转译成C、Python和JavaScript。

Z语言v0.1版包括如下内容：

### 语言特性：
- [x] print
- [x] 字符串常量
- [x] 整数
- [ ] 算数运算
- [ ] 比较运算
- [ ] if语句
- [ ] for循环
- [ ] when分支
- [ ] 常量
- [ ] 变量
- [ ] 幻量
- [ ] 自定义函数
- [ ] 递归函数
- [ ] 自定义类型
- [ ] 方法
- [ ] 动态类型any
- [ ] 编译期函数调用

#### 工具链：

- 解释器：zi
- 编译器：z
    - gas: GNU X86_64汇编
    - masm64: Microsoft Assembly 64bit
- 转译器：
    - z2c
    - z2py
    - z2js
- REPL：zr

## 中长期规划 

### 第一册：基础

#### 第一章：基本框架

1. ~~Hello world~~
1. ~~解释器~~
1. ~~编译器~~
1. ~~REPL~~
1. ~~转译器：C~~
1. ~~转译器：Python~~
1. ~~转译器：JS~~
1. ~~基本函数~~

#### 第二章：基本运算

1. ~~整数~~
1. ~~加法~~
1. ~~减法~~
1. 括号
1. 乘除法
1. ~~单元测试~~
1. 浮点数
1. 自定义函数`pow(m, n)`

#### 第三章：逻辑运算

1. true/false
1. 比较运算（<, >, ==, !=）
1. if语句
1. for语句
1. when语句
1. 递归函数
1. 斐波那契数列

#### 第四章：复合类型

1. 数组
1. 哈希
1. 字符串
1. 自定义类型`class`
1. 动态类型`any`
1. 字典`map`
1. JSON

#### 第五章：面向对象

1. 方法
1. 接口
1. 组合
1. 继承？
1. 运行时多态

### 第二册：生态

#### 第六章：标准库

1. 模块化
1. 面向场景编程`SOP`
1. 导入与导出
1. 数学库：`math`
1. I/O库

#### 第七章：高阶特性

1. 闭包
1. 生成器
1. slice/range
1. 函数式编程
1. 异步

#### 第八章：内存管理

1. 手动内存管理（malloc/free）
1. 引用计数
1. 垃圾回收
1. 内存池
1. 弱引用和借用
1. 生命周期管理
1. 自动引用计数（ARC）
1. 自动内存释放（Auto Free）

#### 第九章：跨语言

1. FFI：C
1. FFI：Python
1. FFI：JS
1. Binding: C
1. Binding: Python
1. Binding: JS
1. c2z
1. py2z
1. js2z
1. bash2z
1. 跨语言REPL

#### 第十章：元编程

1. 编译期脚本
1. 泛型
1. 宏
1. 静态反射
1. 动态反射
1. 代码生成
1. DSL

#### 第十一章：工具链

1. 测试框架
1. 性能工具
1. zb: Z Builder
1. 包管理，repo
1. LSP/IDE插件
1. 社区工具

#### 第十二章：优化

1. AST优化
1. IR
1. SSA
1. Passes
1. JIT


#### 第十三章：打通生态

C生态:

1. HTTP服务
1. redis/数据库访问
1. 图形库
1. GUI库
1. 游戏引擎
1. 多媒体库

Python生态:

1. numpy
1. plot
1. pandas
1. tensorflow
1. pytorch
1. Stable Diffusion

JS生态:

1. 前端GUI（vuejs）
1. wasm
1. webgpu
1. vscode

#### 第十四章：应用展示

1. REPL：zcalc，带有记忆功能的可编程计算器。
1. 编译器：用FFI的形式，调用C语言的库，实现一个最简单的HTTP服务。
1. 转译C：调用SDL库，实现一个最简单的2D游戏，并借用Emscripten转译成WASM。
1. 转译Python：调用pyplot库，绘制一个K线图。
1. 转译JavaScript：调用vuejs库，实现一个最简单的前端页面，并展示上面两个成果。

### 第三册：应用

如果能做到这个地步，Z语言应当已经比较成熟，且打通了C/Python/JS的生态，拥有了完整的应用库了。

这时候就可以开始实现我最初的梦想了：用Z语言开发自己的应用。

我大致有如下几个方向的设想：

1. Zap（Z App Platform），前后端开发无缝链接的UI框架。需要打通C/JS生态。
1. Zeco (Z Editor for Coders)，类似于VSCode的通用编辑器，也是Z语言的官方IDE。主要基于C生态；但还需要实现一个WEB版，因此也需要JS。
1. Zire（Z Interactive REPL Environment），融合bash、python、js的交互环境，提供一站式探索式编程的交互环境。需要打通C/Python生态。
1. Zif (Z Image Fusion)，基于Stable Diffusion的图像处理工具。主要基于Python生态，再加上基于JS的界面。
1. Zaivre（Z AI Virtual Reality Engine，可以读作zavor，/ˈzeɪvə/）, AI虚境引擎。需要C/Python/JS。

Zaivre虚境引擎是我的最终目标，也是我学习并开发Z语言的初衷。
这个引擎需要同时打通C/Python/JS的生态，所以我才会选择它们作为Z语言的目标语言。

这些项目没一个好对付的，所以现在只是一个构思，一个方向，具体怎么做到时候再说，至少要等第二册写好了，Z的基本库都能用了再仔细探讨吧。
