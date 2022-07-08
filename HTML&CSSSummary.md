# HTML&CSS总结

## **HTML**

* 这是一个新建的HTML文档  
    ![base.png](https://s2.loli.net/2022/07/07/TS1FhVIeCuK2a5q.png)  
(1) `<!DOCTYPE html>`:声明文档类型。  
(2) `<html></html>`:`<html>`元素。这个元素包裹了整个完整的页面，是一个根元素，其它元素都嵌套到其中。  
(3) `<head></head>`: `<head>`元素。 这个元素是一个容器，它包含了所有你想包含在HTML页面中但不想在HTML页面中显示的内容。这些内容包括你想在搜索结果中出现的关键字和页面描述，CSS样式，字符集声明等等。  

* `<title></title>`:设置页面标题，出现在浏览器标签上。  
* `<body></body>`:在这里书写你的所有内容代码（文本，图片等）。  
* `<br>`:表示换行。  

### 常见的元素  

* `<h1> ~ <h6>`:一级到六级标题。  
   ![image.png](https://s2.loli.net/2022/07/08/9qszyKuBThC17tg.png)  
   ![image.png](https://s2.loli.net/2022/07/08/4vVRz6mnclOhqYF.png)  

* `<a></a>`:超链接标签。用法:`<a href="https://www.baidu.com">百度</a>`  
  * `href`:表示要跳转去的地址 URL。  

* `<img src="URL" alt="文字">`:表示在页面插入一张图片。
  * `src`:标识图片的路径。
  * `alt`:表示获取图片失败时，显示的文字。  

* `<p></p>`:块级元素，定义段落。  

* `<table></table>`:定义表格。  
  ![image.png](https://s2.loli.net/2022/07/08/gIm9Blwq6rZtWfO.png)  
  ![image.png](https://s2.loli.net/2022/07/08/NDiBuflJswoFGTn.png)  
  * `<tr>`:表示行, `<td>`表示行中的单元, `<th>`是表头的单元（将会加粗显示）。  

* 列表：
  ![image.png](https://s2.loli.net/2022/07/08/SfAwbGcjHVQrthT.png)  
  ![image.png](https://s2.loli.net/2022/07/08/SUMgeaW2Q1VIwNp.png)  
  * 有序列表始于 `<ol>` 标签。每个列表项始于 `<li>` 标签。每列使用数字表示。
  * 无序列表使用 `<ul>` 标签
  * 自定义列表以`<dl>`标签开始。每个自定义列表项以`<dt>`开始。每个自定义列表项的定义以`<dd>`开始。  

* `<div></div>,<span></span>`: `<div>`元素是块级元素，它可用于组合其他 HTML 元素的容器，没有其他意义。 `<span>`元素是内联元素，可用作文本的容器`<span>`元素也没有特定的含义。  

* `<form></form>`:定义表单。  
  ![image.png](https://s2.loli.net/2022/07/08/mvrg9XBcWtAnZeK.png)  
  ![image.png](https://s2.loli.net/2022/07/08/uEsPiWIAUzXfBdG.png)  
  * 文本域通过`<input type="text">`标签来设定，当用户要在表单中键入字母、数字等内容时，就会用到文本域。
  * 标签`<input type="password">`来定义输入密码字段。
  * `<input type="radio">`标签定义了表单的单选框选项。
  * `<input type="checkbox">`定义了复选框。
  * `<input type="submit">`定义了提交按钮。 

## **CSS**  

* CSS语法
CSS 规则由两个主要的部分构成：选择器，以及一条或多条声明，选择器通常是您需要改变样式的 HTML 元素。每条声明由一个属性和一个值组成。属性（property）是您希望设置的样式属性（style attribute）。每个属性有一个值。属性和值被冒号分开。  

* 选择器  
  * id选择器:id 选择器可以为标有特定 id 的 HTML 元素指定特定的样式。HTML元素以id属性来设置id选择器,CSS 中 id 选择器以 "#" 来定义。
  * class选择器:class 选择器用于描述一组元素的样式，class 选择器有别于id选择器。class可以在多个元素中使用。class 选择器在HTML中以class属性表示, 在 CSS 中，类选择器以一个点"."号显示。

* CSS的引入
  * `<link rel="stylesheet" type="text/css" href="mystyle.css">`:`href`表示要引入的样式路径。
  * `<style></style>`:在这里写内部样式。  

* CSS背景  
  * `background-color`:该属性定义了元素的背景颜色
  * `background-image`:该属性描述了元素的背景图像。默认情况下，背景图像进行平铺重复显示，以覆盖整个元素实体。
  * `background-repeat`:使用 `background-repeat` 属性可以让图像不平铺。
  * `background-position`:可以改变图像在背景中的位置。
  * `background-attachment`:背景图像是否固定或者随着页面的其余部分滚动。  

* CSS文本和字体格式  
  * `color`:设置文本颜色
  * `letter-spacing`:可以设置字符间的间距
  * `line-height`:设置行高
  * `text-align`:元素中文本对齐
  * `text-shadow`:设置文本阴影
  * `word-spacing`:设置字间距
  * `font`:声明字体的属性
  * `font-size`:设置字体的大小
  * `font-style`:设置字体的样式

* CSS盒子模型
盒子模型指的是一个 HTML 元素可以看作一个盒子。从内到外，这个盒子是由内容 content, 内边距 padding, 边框 border, 外边距 margin构成的，如下图所示：
![image.png](https://s2.loli.net/2022/07/08/HGqKIoixU4E3OQv.png)
  * `Content`:内容，容器最中心的位置。
  * `Padding(内边距)`:即内容和边框之间的区域。
  * `Border`:边框，默认不显示。
  * `Margin`:外边距，边框以外与其它元素的区域。

* CSS边框和边距  
  * `border-style`:用于设置元素所有边框的样式，或者单独地为各边设置边框样式。
  * `border-width`:用于为元素的所有边框设置宽度，或者单独地为各边边框设置宽度。
  * `border-color`:设置元素的所有边框中可见部分的颜色，或为 4 个边分别设置颜色。
  * `margin`:外边距
    * `margin-bottom`:设置元素的下外边距。
    * `margin-left`:设置元素的左外边距。
    * `margin-right`:设置元素的右外边距。
    * `margin-top`:设置元素的上外边距。
  * `padding`:内边距
    同外边距属性。

* CSS分组和嵌套选择器
  * `p{ }`:为所有 p 元素指定一个样式
  * `.marked{ }`: 为所有`class="marked"`的元素指定一个样式。
  * `.marked p{ }`: 为所有`class="marked"`元素内的`p`元素指定一个样式。
  * `p.marked{ }`: 为所有`class="marked"`的`p`元素指定一个样式。

* 定位  
  * `position`:属性用于对元素进行定位。该属性有以下一些值：
    * static 静态, HTML 元素的默认值，即没有定位，遵循正常的文档流对象。
    * relative 相对,相对定位元素的定位是相对其正常位置。
    * fixed 固定,元素的位置相对于浏览器窗口是固定位置,即使窗口是滚动的它也不会移动。
    * absolute 绝对,元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于`<html>`。

* CSS Overflow
CSS overflow 属性用于控制内容溢出元素框时显示的方式。
  * `visible`:默认值。内容不会被修剪，会呈现在元素框之外。
  * `hidden`:内容会被修剪，并且其余内容是不可见的。
  * `scroll`:内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。
  * `auto`:如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。

* CSS浮动
CSS的Float（浮动），会使元素向左或向右移动，其周围的元素也会重新排列。
Float（浮动），往往是用于图像，但它在布局时一样非常有用。
  * `clear`:指定不允许元素周围有浮动元素。
    * left
    * right
    * both
    * none
  * `float`:指定一个盒子（元素）是否可以浮动。
    * left
    * right
    * none
    * inherit

* 不透明度
我们可以用`opacity`对任何元素（不过常用于图片）设置不透明度。
值在`[0.0～1.0]`之间，值越低，透明度越高。  
