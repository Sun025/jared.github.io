# CSS几种等高布局方式
- Tablebox布局方式
- Flexbox布局方式
- Grid布局方式
- 背景色伪等高方式
- 设置元素内底边距和外底边距大正负数值方式

## 1.Tablebox布局方式
父元素 display:table;
子元素（子项目） display:table-cell
缺点：部分样式属性会被限制

## 2.Flexbox布局方式
父元素：
display:flex;
flex-direction: row

子元素：
flex: 1;(等宽)
或
flex; 0;（自定义宽度）

## 3.Grid布局方式
父元素：
display: grid;
grid-auto-flow: colunm;

## 4.背景色伪等高方式
将父元素的背景色设置为较短的那个元素背景色，形成视觉上的欺骗。
优点：不存在兼容性问题。

## 5.设置元素的内底边距和外底边距大正负数值方式
父元素：
overflow: hidden;（只要能开启BFC都可以）

子元素：
padding-bottom: 9999px;
margin-bottom: -9999px;