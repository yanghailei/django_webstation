# h1> 这是一个HTML的简易教程 </h1>

# HTML 元素 = 开始标签 + 元素内容 + 结束标签

图片
<img src="zmypic.png" width="100" height="150">

链接
<a href="http://www.baidu.com">这是一个链接</a>

段落
<p>这是一个段落。</p>


# Tips
> 即使您忘记了使用结束标签，大多数浏览器也会正确地显示 HTML，因为关闭标签是可选的。”

> HTML 标签对大小写不敏感：P> 等同于 p>。许多网站都使用大写的 HTML 标签。”

> !-- 这是一个注释 -->”

> “如果您希望在不产生一个新段落的情况下进行换行（新行），请使用 br /> 标签：”

> h1> 定义最大的标题。 h6> 定义最小的标题。

> hr>	定义水平线

> 当显示页面时，浏览器会移除源代码中多余的空格和空行。所有连续的空格或空行都会被算作一个空格。需要注意的是，HTML 代码中的所有连续的空行（换行）也被显示为一个空格。

> a href="/" target="_blank">访问 ziqiangxuetang.com! /a> 如果你将 target 属性设置为 "_blank", 链接将在新窗口打开

> id属性可用于创建在一个HTML文档书签标记。书签是不以任何特殊的方式显示，在HTML文档中是不显示的，所以对于读者来说是隐藏的。

> title> - 定义了HTML文档的标题 | 使用 title> 标签定义HTML文档的标题

> base> - 定义了所有链接的URL | 使用 base> 定义页面中所有链接默认的链接目标地址。

> meta> - 提供了HTML文档的meta标记 | 使用 meta> 元素来描述HTML文档的描述，关键词，作者，字符集等。

```
通常标签 <strong> 替换加粗标签 <b> 来使用, <em> 替换 <i>标签使用。
然而，这些标签的含义是不同的：
b> 与 i> 定义粗体或斜体文本。
strong> 或者 em>意味着你要呈现的文本是重要的，所以要突出显示。现今所有主要浏览器都能渲染各种效果的字体。不过，未来浏览器可能会支持更好的渲染效果。
```

```
<head> 元素包含了所有的头部标签元素。在 head>元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种meta信息。
可以添加在头部区域的元素标签为: title>, style>, meta>, link>, script>, noscript>, and base>.
```






# HTML 属性
1. HTML 元素可以设置属性
2. 属性可以在元素中添加附加信息 about an element
3. 属性一般描述于开始标签
4. 属性总是以名称/值对的形式出现，比如：name="value"。

|属性	 | 描述|
| ------------- |:-------------------:|
|class	 |为html元素定义一个或多个类名（classname）(类名从样式文件引入)|
|id | 定义元素的唯一id|
|style |	规定元素的行内样式（inline style） title text 规定元素的额外信息（可在工具提示中显示）|
|title | 描述了元素的额外信息 (作为工具条使用)|

# title> 元素:
1. 义了浏览器工具栏的标题
2. 当网页添加到收藏夹时，显示在收藏夹中的标题
3. 显示在搜索引擎结果页面的标题

# meta> 元素
1. meta标签描述了一些基本的元数据。
2. meta标签提供了元数据.元数据也不显示在页面上，但会被浏览器解析。
3. META元素通常用于指定网页的描述，关键词，文件的最后修改时间，作者，和其他元数据。
4. 元数据可以使用浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他Web服务。
5. <meta>一般放置于 <head>区域

# HTML head 元素
|标签	|描述|
| ------------- |:--------------------------------:|
| head	| 定义了文档的信息 |
| title	| 定义了文档的标题 |
| base	| 定义了页面链接标签的默认链接地址 |
| link	| 定义了一个文档和外部资源之间的关系 |
| meta	| 定义了HTML文档中的元数据 |
| script	| 定义了客户端的脚本文件 |
| style	| 定义了HTML文档的样式文件 |

为搜索引擎定义关键词:
> meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">

为网页定义描述内容:
> meta name="description" content="Free Web tutorials on HTML and CSS">

定义网页作者:
> meta name="author" content="Hege Refsnes">

每30秒 刷新一次当前页面:
> meta http-equiv="refresh" content="30">


# 内部样式表
> 当单个文件需要特别样式时，就可以使用内部样式表。你可以在 head> 部分通过 style>标签定义内部样式表:
```html
<head>
<style type="text/css">
body {background-color:yellow;}
p {color:blue;}
</style>
</head>
```
# 外部样式表
> 当样式需要被应用到很多页面的时候，外部样式表将是理想的选择。使用外部样式表，你就可以通过更改一个文件来改变整个站点的外观。
```html
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

# 在 HTML 中，图像由img> 标签定义。img> 是空标签，意思是说，它只包含属性，并且没有闭合标签。
要在页面上显示图像，你需要使用源属性（src）。src 指 "source"。源属性的值是图像的 URL 地址。
alt 属性用来为图像定义一串预备的可替换的文本。替换文本属性的值是用户定义的。
URL 指存储图像的位置。
在浏览器无法载入图像时，替换文本属性告诉读者她们失去的信息。此时，浏览器将显示这个替代性的文本而不是图像。为页面上的图像都加上替换文本属性是个好习惯，这样有助于更好的显示信息，并且对于那些使用纯文本浏览器的人来说是非常有用的。
定义图像的语法是：
```html
<img src="url" alt="some_text">
```
p style="font-family:arial;color:red;font-size:20px;">A paragraph.</p>
h2 style="background-color:red;">This is a heading</h2>
h1 style="text-align:center;">Center-aligned heading</h1>

# HTML 表格
表格由 table> 标签来定义。每个表格均有若干行（由 tr> 标签定义），每行被分割为若干单元格（由 td> 标签定义）。字母 td 指表格数据（table data），即数据单元格的内容。数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等。/p>。表格的表头使用 <th> 标签进行定义。
```html
<table border="1">
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>row 1, cell 1</td>
    <td>row 1, cell 2</td>
  </tr>
  <tr>
    <td>row 2, cell 1</td>
    <td>row 2, cell 2</td>
  </tr>
</table>
```


# HTML无序列表
无序列表是一个项目的列表，此列项目使用粗体圆点（典型的小黑圆圈）进行标记。无序列表使用 li> 标签
```html
<ul>
  <li>Coffee</li>
  <li>Milk</li>
</ul>
```
# HTML 有序列表
同样，有序列表也是一列项目，列表项目使用数字进行标记。 有序列表始于 ol> 标签。每个列表项始于 li> 标签。列表项项使用数字来标记。
```html
<ol>
<li>Coffee</li>
<li>Milk</li>
</ol>
```

# HTML 自定义列表
自定义列表不仅仅是一列项目，而是项目及其注释的组合。自定义列表以 dl> 标签开始。每个自定义列表项以 dt> 开始。每个自定义列表项的定义以 dd> 开始。
```html
<dl>
  <dt>Coffee</dt>
    <dd>- black hot drink</dd>
  <dt>Milk</dt>
    <dd>- white cold drink</dd>
</dl>
```
# HTML 脚本
noscript> 标签提供无法使用脚本时的替代内容，比方在浏览器禁用脚本时，或浏览器不支持客户端脚本时。noscript>元素可包含普通 HTML 页面的 body 元素中能够找到的所有元素。只有在浏览器不支持脚本或者禁用脚本时，才会显示 <noscript> 元素中的内容：
```html
<script>
document.write("Hello World!")
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```





