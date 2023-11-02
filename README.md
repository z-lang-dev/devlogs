# Z语言炼成记

## 介绍

Z语言是一门面向个人的，用于学习和探索的编程语言。

Z语言着力于编译器相关知识的学习和分享，注重内容的广度，深度上则是由浅及深。

Z语言的实现放在[gitee.com/z-lang/zc](https://gitee.com/z-lang/zc)工程里。

《Z语言炼成记》这本书用来记录我在设计和开发Z语言过程中产生的思考和经历，希望能够让大家更有临场感地去了解Z语言。

我打算采用日志的形式来记录，每做一部分代码，就更新一节。
但我并不能保证每天都有更新，毕竟编译器这种非常繁杂的工作，不可能每天都有值得分享的产出。

话题的形式确定为“一天以内能解决的问题”，如果不能，就分成好几篇。

关于Z语言的更多介绍，可以参看：[Z语言是什么](./Z语言是什么.md) 一节。

## 目录

#### 引言

- [Z语言是什么](./Z语言是什么.md)。

#### 第一章：基本框架

- [最简单的Z程序](./最简单的Z程序.md)。
- [最简单的编译器](./最简单的编译器.md)。

## 短期规划

2023年11月目标：一个可用的玩具语言，同时支持动态解释、静态编译，还能够转译成C、Python和JavaScript。

Z语言v0.1版：
- 语言特性：
    - 基本类型：整数、布尔、字符串
    - 运算：算数运算、比较运算
    - 量值：常量、变量、幻量
    - 语句：if、for、when
    - 函数：自定义函数、函数调用
    - 类型：自定义类型、方法、动态类型any
    - 元编程：编译期函数调用
- 工具链：
    - 解释器：zi
    - 编译器：zc，目标：GNU x86-64汇编
    - 转译器：Z2C、Z2PY、Z2JS
    - REPL：zr

## 中长期规划 

#### 第一章：基本框架

1. Hello world
1. 解释器
1. 编译器
1. REPL
1. 转译器：C
1. 转译器：Python
1. 转译器：JS
1. 基本函数

#### 第二章：基本运算

1. 整数
1. 加法
1. 减法
1. 括号
1. 乘除法
1. 单元测试
1. 浮点数
1. 自定义函数`add(a, b)`

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


#### 第六章：标准库

1. 模块化
1. 面向场景编程`SOP`
1. 导入与导出
1. FFI：C
1. FFI：Python
1. FFI：JS
1. 数学库：`math`
1. I/O库

#### 第七章：高阶特性

1. 闭包
1. 生成器
1. slice/range
1. 函数式编程
1. 异步

#### 第八章：元编程

1. 编译期脚本
1. 泛型
1. 宏
1. 静态反射
1. 动态反射
1. 代码生成
1. DSL

#### 第九章：生态

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

最终产品：zaivre（Z AI Virtual Reality Engine，可以读作zavor，/ˈzeɪvə/）, 一款AI虚境引擎。
