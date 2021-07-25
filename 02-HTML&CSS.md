# 02-HTML&CSS

## HTML 课堂笔记
### 1. Web三门语言： HTML CSS JavaScript
- HTML内容 Content Structure
- CSS装饰 Content Presentation
- JavaScript交互

### 2. 打开一个网页的流程：相当于下载一个app

### 3. HTML: HyperText Markup Language, mockup language but is Not a programming language (图灵不完备)

### 4. JavaScript fatigue：所有框架等最后都会转变回HTML CSS JavaScript

### 5. HTML学习网站： W3School，MDN， 需要时可经常查

### 6. HTML文件结构: 
- 在HTML文件中输入 html:5,按tab键后，自动生成代码
- <DOCTYPE> Document type declaration 声明文件类型
- <html>: 包含head和body
- <head>: 包含meta data (configuration)，title等
- <body>: 内容

### 7. 浏览器打开html的方式:
- 直接打开
- live-server插件: 命令行安装 ```npm install -g live-server```

### 8. Dev Tool: 通过option+command+i快捷打开
- 可以在Dev Tool中的console中直接写Javascript代码
- 技巧：可以直接在Dev Tool中看一些源码，借鉴到自己项目
- Network：可以看到请求记录
- Performance：页面的性能
- Memory：使用的内存
- Application：包含Local Storage，Session，Cookie
- Security：协议等
- LightHouse：整体的performance，SEO，Accessibility等的分析
- 可选择安装的插件：devtools axe-core extension

### 9. Accessibility：可以让更多的用户使用网站，例如视力有障碍的人。例如如果图片缺少alt属性，screen reader无法读出图片。

### 10. SEO：Search Engine Optimization搜索引擎优化: 如何提高网站在有关搜索引擎内的排名
- head metadata可以被搜索引擎读取，也可以被社交网站分享
- 性能好
- 流量高

### 11. HTML tag分为两种: 各种标签可以在w3school和MDN搜索到，使用正确的标签对SEO有益
- block element: `<div> <header> <main>`
    - i: 占据整行
    - ii: 上下有空间

- inline element: <span> 等
    - i: 不会换行，默认在同一行中
    - ii: 上下不占空间

### 12. 常用tag:
- h1, h2, h3, h4, h5, h6: h1每个配置里只能有一个，有层级关系，需要依次使用，不能挑选使用，搜索引擎SEO会注重这一点
- `<p>`: Paragraph 很常用
- `<b> <strong> <i> <em> <mark> <small> <del> <ins>`: Text - Format element格式调整，但大多标签最好不使用，因为在不同浏览器中可能有不同效果，因此要用css实现。除`<strong>`有语义以外。
- `<br>`: 换行
- `<span>`: 可使用span圈中某部分，再用css添加效果，本身不带有style
- `<ul> <ol> <li>`: list标签。ul (unsorted list) ol (ordered list)。会在navigation bar中使用
- `<table>`: 表。一般不会直接用html写，会通过React等framework写。
- `<div>`: default block element
- `<a>`: Link。包含target，_blank在新标签页打开
- `<img>`: 图片。要加alt，对图片的描述。可以用height width调整，但更多要用CSS调整。建议技巧：将图片作为一个background-image放在一个<div>中。
- `<form> <input> <select> <textarea>`: 不再在html中使用，通过JavaScript异步实现。<input>要对应一个<label>会在测试中使用。
- `HTML5 <input>`: require, type可以对input的内容制定输入规则
- `<audio> <video>`: 很少使用通过html做，播放音乐，视频。
- `<!— —>`: comment，主要用于解释一些比较复杂的business logic
- caniuse.com：Browser Compatibility。查询哪些浏览器支持哪些tag。

### 13. File path 文件路径:
- `../` （相对路径）退到上一层目录
- `./` （相对路径）当前目录
- `/`（绝对路径）从root开始
- 绝对路径使用更多

### 面试：
coding test：programing面试一定要和面试官交流，无论是不是pair programming，都要说出自己的思路。


## CSS 课堂笔记

### 1. What is CSS
- 把html当成一个内容，展示由css来完成

### 2. How CSS works 
- Load html源码->浏览器阅读后形成带层级关系的解析->构成dom node， dom tree
- Parse html 过程中：读取css 源码->attach css style到 找到的html dom node

### 3. CSS如何和HTML写到一起：
- inline style: HTML tag中有个style的attribute，可以在style中写。但杂糅了HTML和CSS，难维护，无法复用，最不推荐。
- 在head中加`<style>`，也是杂糅HTML和CSS
- 在head中加`<Link>`，link到CSS文件，在HTML读取tag时会读取到相应CSS信息，最推荐做法。

### 4. CSS selector:
- Simple selector: 元素类型, class, id. class可以多次使用，id只能用一次。
- Attribute selector: 通过条件选取。
- Psuedo selector: 在某种效果下加效果。如hover: a。要与伪元素区别（psuedo elements）例如 p::before.
- universal (*)全局 可能被覆写。Descendant。Child。 

### 5. block element的盒子模型
- `padding`是指与边缘的距离
- `border`边缘
- `margin`与其他元素的距离

### 6. units
- `px` 像素是一种绝对单位，指定的值不会变化
- `%` 相对单位，会在responsive中用到
- `vh vw`占视窗的大小
- `auto 0` 很早之前水平居中等使用
- `em rem` 基于字体大小，em继承父元素大小，rem直接找到最原始的大小

### 7. normalize.css 用于初始化所有css，会在开发中导入，避免出现浏览器差异。

### 8. learnlayout.com 练习CSS定位

## 作业：

- Card Design 用基本的css画出card，把css单独写出。

- SVG怎么用。直接在SVG内部改颜色可以不用CSS改。

- BEM命名方法对class命名。Block-Element-Modifier
