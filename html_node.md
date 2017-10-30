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

### `<big>`

定义较大文本，支持部分标准属性和事件属性。在HTML5中已废弃。




