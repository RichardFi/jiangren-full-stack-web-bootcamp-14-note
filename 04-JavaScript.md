# 02-JavaScript

## JavaScript 课堂笔记

### 面试经验：
- 澳洲的开发更需要横向的经验
- 从旧版本ES6之前开始学，更基础

### 1. JavaScript是什么
- 动态dynamic，弱类型weakly typed语言
- 在之前只运行在浏览器里
- 有了nodejs之后即可在前端也可在后端使用

### 2. JavaScript的特点
- 不是直接从上到下运行代码，而是获得被声明的变量
- 变量声明如果在`function`里, 它会自动提升到`function`的头部，变量声明如果不在`function`里, 它会自动提升到文件的头部
- `'use strict'`自动注入JavaScript，严格模式

### 3. 命名规则
- UPPERCASE, camelCase, PascalCase, under_score
- 不能以数字和符号开头
- 有一些保留词例如if else

### 4. 数据类型
- number
- string 字符文本
- boolean (true, false)
- null 空值
- 复杂数据类型：object，数组

### 5. 运算符
- `+ - * /` 数组合并也用+
- `=` 赋值 
- `== ===` 相等，返回boolean。对相同内容的复杂数据类型用`===`比较会不相等。在应用中只使用`===`
- `! !==` 非，不等 

### 一个JavaScript核心开发者的博客overeacted.io 

### 6. 数组
- 按次序排列的一组值
- 可用index访问或填改数组
- 有各种操作方法push pop
- 很灵活，可以多层，可以存储对象，可以存储其他array

### 7. 条件判断
- if else
- 三元运算 `?expr1 : expr2` 不建议嵌套 可读性相对差

### 8. 循环loop
- `for`循环 `while`循环
- 循环可嵌套
- `break`可以跳出循环，`continue`用于终止本轮循环

### 面试：
- 面试时被问如何学习：podcast (syntax, software daily), udemy, front-end master, side project, 参加meet up

### 9. Function
- `return`表示返回
- JavaScript会直接返回 `return` 的值，之后的语句不会执行
- 闭包closure，当function嵌套时，inner function acesss outside，function里可以使用外部变量，外部不能用function内部的变量。需要慢慢理解。
- function中this的使用

### 10. DOM Document Object Model
- 是JavaScript操作网页的接口，将网页变为JS进行操作。
- 将HTML解析成一系列的节点，再由这些节点组成一个树状结构
- 现在基本不再直接用了
- React已经接管DOM操作了（虚拟DOM）

### 作业
- 无
- 多练习，再看看闭包和this的内容