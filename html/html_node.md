# HTML 标签

## 基础标签

### `<!DOCTYPE>`

```html
<!DOCTYPE html> <!--HTML5声明-->
```

位于文档前，不属于HTML标签，用来告诉浏览器HTML的版本。

### `<html>`

```html
<html manifest="URL" ...> <!--支持全局属性-->
```

对于`manifest`(5NEW)属性，用来指定文档的缓存位置。可以是另一个网站，也可以网站内的某个文件。

### `<title>`

```html
<title ...>  <!--支持全局属性-->
```

文档标题，使用在头部。

### `<body>`

```html
<body ...>  <!--支持全局属性和事件属性，在HTML5中删除了呈现属性-->
```
呈现属性指的是指定文档body的背景色，链接颜色等的属性。

### `<h1>`

```html
<h1 ...>  <!--支持全局属性和事件属性，在HTML5中删除了align属性-->
```
align属性指的是标题的排列方式，靠左靠右等。

### `<br>`

```html
<br ...>  <!--支持全局属性和事件属性，没有结束标签-->
```

### `<hr>`

```html
<hr ...>  <!--支持全局属性和事件属性，在HTML5中删除了呈现属性-->
```

呈现属性就是颜色，宽度，高度以及排列方式的设定。

### `<!---->`

```html
<!--这是一个注释-->  <!--不支持标准属性和事件属性-->
```

## 文本格式

### `<acromym>`

只取首字母缩写，HTML5中已经废弃。

```html
Can I get this <acronym title="as soon as possible">ASAP</acronym>?
```

### `<abbr>`

定义一个缩写，和上面标签业务类似。支持全局属性和事件属性。

```html
The<abbr title="World Health Organization">WHO</abbr> was founded in 1948.
```

### `<address>`

定义一个地址，通常显示为斜体，大多数浏览器会自加换行。常位于`<footer>`中。支持全局属性和事件属性。

```html
<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```

### `<b>`

显示粗体文本，作为最后选择的标签。支持全局属性和事件属性。

```html
<p>这是一个普通的文本- <b>这是一个加粗文本</b>。</p>
```

### `<bdi>`

将一段文字从父元素中隔离显示。z支持全局属性和事件属性。

```html
<ul>
 <li>用户 <bdi>hrefs</bdi>: 60 分</li>
 <li>用户 <bdi>jdoe</bdi>: 80 分</li>
 <li>用户 <bdi>إيان</bdi>: 90 分</li>
</ul>
```

### `<bdo>`

覆盖默认的文本方向，必须和`dir`属性一起使用。支持全局属性和事件属性。

```html
<p><bdo dir="rtl">该段落文字从右到左显示。</bdo></p>
```

### `<big>` `<small>`

定义较大文本和较小文本，支持部分标准属性和事件属性。在HTML5中已废弃`big`。

### `<blockquote>` `<cite>`

前者用来定义引用文本，后者标注作品的标题。支持全局属性和事件属性。

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
</blockquote>
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>
```
### `<code>` `<samp>`

用来定义计算机代码和代码样本格式。支持全局属性和事件属性。

### `<dfn>`

用来定义项目格式。支持全局属性和事件属性。

### `<font>`

定义文本的字体，尺寸和颜色，HTML5已经废弃。

```html
<font face="verdana" color="green">这是一些文本!</font>
```

### `<em>` `<strong>`

定义强调文本，支持全局属性和事件属性。

### `<i>`

定义斜体文本。斜体文本是左后使用的语义元素。

### `<ins>` `<u>` `<del>` `<strike>` `<s>`

定义插入文本下划线文本和删除文本，以及加删除线的文本（HTML5已废弃strike）。支持全局属性和事件属性。

```html
<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>
```

### `<kbd>`

定义键盘输入文本。支持全局属性和事件属性。

### `<mark>`

定义带有记号的文本。

```html
<p>Do not forget to buy <mark>milk</mark> today.</p>
```

### `<meter>`

定义度量的标签。支持全局属性和事件属性。说明一下新增属性的含义：

|属性|说明|
|---|
|form|指定元素所属表单，值为id|
|high|指定高的范围|
|low|指定低的范围|
|max|指定大的范围|
|min|指定小的范围|
|optimum|规定度量的最优值|
|value|必须，固定度量的当前值|

```html
<meter value="2" min="0" max="10">2 out of 10</meter><br>
<meter value="0.6">60%</meter>
```

### `<pre>`

预格式化文本，不会格式化诸如空格换行之类的信息。支持全局属性和事件属性。

注意`width`属性在HTML5中已经被废弃。

```html
<pre>
此例演示如何使用 pre 标签
对空行和 空格
进行控制
</pre>
```

### `<progess>`

定义任务进度。支持全局属性和事件属性。另外：

`max`和`value`属性分别指定最大值和当前值。

```html
<progress value="22" max="100"></progress>
```

### `<q>`

段语句的引用。


### `<ruby>` `<rp>` `<rt>`

定义ruby注释和定义不支持ruby的浏览器所显示的内容。以及注音。

```html
<ruby>
  漢 <rp>(</rp><rt>han</rt><rp>)</rp>
  字 <rp>(</rp><rt>zi</rt><rp>)</rp>
</ruby>
```

### `<sub>` `<sup>`

定义下标和上标文本。

```html
<p>这个文本包含 <sub>下标</sub>文本。</p>
<p>这个文本包含 <sup>上标</sup> 文本。</p>
```

### `<time>`

定义一个时间文本，属性`datetime`规定日期和时间。

```html
<p>我在 <time datetime="2016-02-14">情人节</time> 有个约会。</p>
```

### `<wbr>`

定义分行位置，在浏览器窗口变小时自动分行。

### `<tt>`

定义打印文本，HTML5已经废弃。

### `<var>`

定义文本的变量部分。

## 表单

一共13个标签和表单有关，涉及输入控件，输出控件以及样式控件等。

### `<form>`

表单根标签，支持全局属性和事件属性，同时还有自己的属性：

|属性|值|说明|
|---|
|accept|MIME_type|服务器收到文件的类型（在上传文件时使用）HTML5以废弃|
|accept-charset|character-set|规定表单数据字符集|
|action|URL|规定表单向服务器提交的位置|
|autocomplete|on off|是否自动填充表单|
|enctype|...|在向服务器发送数据之前的编码方式，适用于post情况|
|method|get post|规定提交表单的HTTP方法|
|name|text|表单的名称|
|novalidate|novalidate|如果使用该属性，在提交表单时就不会对表单进行验证|
|target|_blank _self _parent _top|规定在何处打开action URL|

### `<input>`

输入标签。有自己的属性。

|属性|值|说明|
|accept| MIME_type|规定上传文件的类型（只针对type为file）|
|align|left right top bottom middle|规定图像的对齐方式，HTML5已弃用|
|alt|text|规定图像输入的替代文本|
|autocomplete|on off|规定字段是否自动填充|
|checked|checked|规定预选的元素（只针对type为checkbox和radio）|
|disabled|disabled|是否禁用该输入元素|
|form|form_id|该输入元素使用那个表单|
|formaction|URL|规定提交处理控件文件的URL，只针对type为image和submit|
|formenctype|...|在向服务器发送数据之前的编码方式，适用于post情况|
|formmethod|get post|规定发送表单数据到action URL的方法，只针对type为image和submit|
|formnovalidate|formnovalidate|覆盖表单的novalidate属性|
|formtarget|_blank _self _parent _top framename|提交表单后的响应名称或关键词。只针对type为image和submit|
|height|pixels|高度，只针对image type|
|width|pixels|宽度，只针对image type|
|list|datalist_id|引用datalist元素|
|max|number date|规定元素的最大值|
|min|number data|规定元素的最小值|
|maxlength|number|规定允许最大字符数|
|mutiple||启动该属性就允许用户向input元素输入多个值|
|name|元素名称|
|pattern|regexp|验证输入的正则表达式|
|placeholder|text|描述输入字段预期值的提示信息|
|randonly||规定字段只读|
|required||规定必须输入的字段|
|size|number|元素以字符计数的可见宽度|
|src|URL|提交按钮的图像的URL，仅支持type为image|
|step|number|合法数字间隔|
|type|button checkbox color date datetime datetime-local email file hidden image month number password radio range reset search submit tel text time url week|输入元素类型|
|value|text|value值|
