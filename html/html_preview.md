# HTML 学习指导（HTML5标准）

## 简介

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>HTML实例</title>
</head>
<body>
  <h1>标题</h1>
  <p>段落</p>
</body>
</html>
```
`<!DOCTYPE html>`声明文档性质。`<html>`根元素。`<head>`包含文档元数据和标题。依次类推理解。

HTML由标签（或元素）组成。HTML文件需要浏览器渲染，浏览器只会显示`<body>`标签内内容。

通用声明用来声明文档的版本号等内容。

## HTML元素

HTML元素由起始标签，元素内容，闭合标签构成。
起始标签必须存在，闭合标签非必须，当时建议写作规范。
元素内容可以为空。
大多数元素可以拥有*属性*。
元素可以嵌套使用。
元素标签对大小写不敏感。

## HTML属性

HTML属性用来给元素添加附加信息。
HTML属性一般写在起始标签中。
HTML属性总是以键值对形式出现。
HTML属性和属性值对大小写不敏感。推荐使用小写属性和属性值。

## HTML标题

标题一共定义了6级。
标题的意义不仅在外观上，还在整个文档结构上。
使用`<hr>`可以添加水平线。

## HTML段落

浏览器会自动在段落前后添加空行。
如果不希望产生一个新段落而换行，请使用`<br>`。
注意，段落和显示效果和浏览器相关，多个空格和多个空行可能被转换为一个空格。

## 文本格式化

|标签|效果|
|---|
|`<b>` `<strong>`|粗体|
|`<i>` `<em>`|斜体|
|`<big>` `<small>`|大小|
|`<sup>` `<sub>`|上下标|
|`<ins>` `<del>`|插入和删除|
|`<code>`|计算机代码|
|`<kbd>`|键盘码|
|`<samp>`|计算机代码样本|
|`<var>`|变量|
|`<pre>`|预格式文本，可以避免多空格被浏览器格式化|
|`<abbr>`|缩写|
|`<address>`|地址|
|`<q>` `<cite>`|引用|

## HTML链接

```html
<a href="www.baidu.com">baidu.com</a> <!--超链接-->
<a id="top">TOP</a>
<a href="#top">to TOP</a> <!--锚点-->
```
超链接不仅仅是网站的，还能是锚点，或者表示意图的字符串，比如发送邮件给某人等。

## HTML `<head>`

HTML头部分可以插入7种标签。

|标签|作用|
|---|
|`<title>`|标题|
|`<base>`|基本链接地址|
|`<link>`|表明文档与外部文件关系，通常用于链接到样式表|
|`<style>`|定义文档样式文件引用地址|
|`<meta>`|元数据|
|`<script>`|加载脚本文件|

## HTML CSS
在HTML中引用CSS，详见CSS部分。

## HTML 图像

```html
<img src="..." alt="...">
```

## HTML 表格

|标签|说明|
|---|
|`<table>`|表格|  
|`<tr>`|行|
|`<th>`|表头|
|`<td>`|列|
|`<caption>`|标题|
|`<colgroup>`|列的组|
|`<col>`|列的属性|
|`<thead>`|页眉|
|`<tbody>`|主体|
|`<tfoot>`|页脚|


## HTML 列表

HTML列表分为无序列表，有序列表和自定义列表。

|标签|说明|
|---|
|`<ul>`|无序列表|
|`<ol>`|有序列表|
|`<li>`|列表项|
|`<dl>`|定义列表|
|`<dt>`|列表项目|
|`<dd>`|项的描述|

## HTML 区块元素

区块元素，以新行开始：

```html
<h1> <p> <ul> <table>
```

内联元素，接着开始：

```html
<a> <b> <td> <img>
```

## HTML 布局

使用`<div>`或`<table>`对HTML分区布局。

## HTML 表单

使用`<form>`和`<input>`的一系列组合完成表单的创建。包括下拉菜单。

|标签|说明|
|---|
|`<form>`|表单|
|`<input>`|输入域|
|`<textarea>`|文本域（多行输入控件）|
|`<label>`|input元素标签|
|`<fieldset>`|一组表单的外框|
|`<legend>`|field的标题|
|`<select>`|下拉选项列表|
|`<optgroup>`|定义选项组|
|`<option>`|下拉列表中的选项|
|`<button>`|按钮|
|`<datalist>`|预先定义的输入控件选项列表|
|`<keygen>`|表单密钥生成器字段|
|`<output>`|计算结果|

## HTML 框架

通过`<iframe>`标签实现html嵌套。

## HTML 颜色

使用`#111111`或`rgba(r,g,b,a)`来实现颜色的表示。

## HTML 脚本

|标签|说明|
|---|
|`<script>`|定义客户端脚本|
|`<noscript>`|当脚本不可用时的替代|

## HTML 字符实体

由于HTML的部分字符被保留，在输入这些字符时需要单独处理。

## HTML5 Canvas

`<canvas>`是一块画布，可以使用`<style>`或脚本绘制内容。

## HTML5 SVG

SVG是使用XML描述2D图形的语言。`<svg>`。

## HTML5 MathML

`<math>`是一种格式化数学公式的标签。

## HTML5 拖放实现

//TODO
HTML5的拖放依赖js脚本实现。实现会在js中说明。