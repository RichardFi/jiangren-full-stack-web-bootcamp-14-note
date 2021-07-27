# 03-CSS&SASS.md

## SASS

### 1. SASS是CSS的superset
- 一种对CSS的改造
- 不是替换
- 被浏览器读取时会被编为CSS
- 针对CSS问题进行改造
    - CSS可复用性不高
    - CSS不具备逻辑
    - CSS的模块化不好
- Pre-CSS

### 2. SASS的安装 `npm install sass -g`
- 用`sass styles.scss style.css`编译CSS

### 3. SASS
- 可用`$primary-color:red;`创建变量
- `@import theme` 载入, 可直接使用变量
- `@use theme` 使用变量时要用`theme.primary-color`
- 可以直接在
- 可以把一个部分的内容全写在一起，易读
- `@mixin` 可以实现复用，相当于一个function
- `% @extend` 简单复用
- 数值可以做计算
- 课程中都默认用sass

### 4. Flexbox一个display的属性
- flex-item
- flex-container
- https://css-tricks.com/snippets/css/a-guide-to-flexbox/

### 5. CSS library 例如Boostrap
- 导入就像导入一个css文件一样
- 使用他写好的class，直接导入
- 推荐library tailwindcss

### 6. Material Design - design language
- 有些library有design language (e.g. material ui)，有些没有 (e.g. Boostrap)

### 7. Consistency一致性
- Typo字体
- 颜色
- Spacing and Positioning


## 作业
- 3-5个cards，内部用flexbox做
- 外部可以用grid system
- 尽量不用position
- 体会一下什么时候用grid，什么时候用flexbox
- 读一下design language例如AntD