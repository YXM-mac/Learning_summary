# **HTML**

## **㈠HTML入门**

----------

### **HTML的定义**

  HTML，超文本标记语言，写给浏览器的语言，目前网络上应用最广泛的语言。HTML也在不断的更新，最新版本已经出现了HTML5。在HTML5中出现了许多新特性，也遗弃了一些旧元素。我们写好html文件后，在浏览器中打开。主流的浏览器包括IE、Firefox、Chrome、Goole等。

HTML 是用来描述网页的一种语言。  

* HTML 指的是超文本标记语言 (Hyper Text Markup Language)  
* HTML 不是一种编程语言，而是一种标记语言 (markup language)  
* 标记语言是一套标记标签 (markup tag)  

### **HTML 编辑器**

* Sublime Text 3
* WebStorm



## **㈡ HTML文档结构**

----------

### **HTML文档基本结构**


```html

DTD(Document Type Definition)  -------------- 文档定义类型
<html>  -------------- 文本描述网页
    <head>  -------------- 文档头部标记：含脚本，样式表等等。
        <meta />   -------------- 定义文档字符集、使用语言、作者等基本信息
        <title>标题</title>  -------------- 定义文档的标题
    </head>
    <body>   -------------- 网页主体,是可见的页面内容
        <h1>Hello world</h1> -----------标题
    </body>
</html>
```

* &lt;body&gt; 与 &lt;/body&gt; 之间的文本是可见的页面内容
* &lt;head&gt;与&lt;/head&gt;头部元素的容器：
* &lt;head&gt; 定义关于文档的信息。

    *  &lt;head&gt; 定义关于文档的信息。
		&lt;title&gt; 定义文档标题。
		&lt;base&gt; 定义页面上所有链接的默认地址或默认目标。
		&lt;link&gt; 定义文档与外部资源之间的关系。
		&lt;meta&gt; 定义关于 HTML 文档的元数据。
		&lt;script&gt; 定义客户端脚本。
		&lt;style&gt; 定义文档的样式信息。

例子:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> 
<html xmlns="http://www.w3.org/1999/xhtml"> 
<head> 
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" /> 
	<title>制作我的第一个网页</title> 
</head> 
<body> 
	<h1>Hello world</h1>
</body> 
</html>
```

在上面的例子中，第一个标签&lt;html&gt; 是告诉浏览器这是html文档的开始。Html文档的最后一个标签是&lt;/html&gt; ，是告诉浏览器这是html的终止。标签&lt;head&gt; &lt;/head&gt; 之间的文本是头部信息，在&lt;title&gt; &lt;/title&gt; 之间的文本是文档标题，会显示在浏览器的窗口的标题栏。&lt;body&gt; &lt;/body&gt; 之间的文本是正文。

### **HTML 文档类型**

* &lt;!DOCTYPE&gt; 声明必须是 HTML 文档的第一行，位于 &lt;html&gt; 标签之前。
* 作用：指示浏览器关于页面使用哪个 HTML 版本进行编写的指令。

```html
//HTML 5
<!DOCTYPE html>

//HTML 4.01 Strict
该 DTD 包含所有 HTML 元素和属性，但不包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">

//HTML 4.01 Transitional
该 DTD 包含所有 HTML 元素和属性，包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" 
"http://www.w3.org/TR/html4/loose.dtd">

//HTML 4.01 Frameset
该 DTD 等同于 HTML 4.01 Transitional，但允许框架集内容。
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" 
"http://www.w3.org/TR/html4/frameset.dtd">

//XHTML 1.0
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```
### **规范的html页面**

##### **1、文档声明**

在<html>前，要写文档声明语句: <!DOCTYPE HTML>，当然也可以用小写表示。文档声明的作用是告诉浏览器该文档遵循html规范。

##### **2、标题**

一般情况下，我们都会设定html文档的标题。这样的作用是使用户看起来感觉友好。标签为<title></title>,标签内放标题名称。

##### **3、页面编码**

编码的种类有多种，但常用的是utf-8和gb2312。utf-8为多国语言编码，gb2312为中文简体编码。对于编码的详细问题，可以浏览博客。设置网页编码的语句为<meta charset= "utf-8" />，是在<head></head>标签内定义的。

##### **4、页面关键字，内容**

我们可以在文档中设置一些关键词，内容介绍。这样的好处是，当我们的网页发布在网上，用户可以通过在搜索框中输入关键字，找出一些比较符合的网页。这样一来，我们的网页便可以更容易地被别人访问。



### **HTML 标记标签**

HTML 标记标签通常被称为 HTML 标签 (HTML tag)。

* HTML 标签是由尖括号包围的关键词，比如  &lt;html&gt;

* HTML 标签分为单标记和双标记：
	* 单标记：&lt;标记名称 属性名称="属性值" ... /&gt;，比如 &lt;br/&gt;
	* 双标记：&lt;标记名称 属性名称="属性值" ... &gt;&lt;/标记名称&gt;，比如 和 ；第一个标签是开始标签，第二个标签是结束标签。

### **HTML 属性**

* 属性总是以名称/值对的形式出现，比如：name="value"。

* 属性总是在 HTML 元素的开始标签中规定。

* 属性值应该始终被包括在引号内。双引号是最常用的，不过使用单引号也没有问题。

```html
属性    值&描述
class    规定元素的类名（classname）
id         规定元素的唯一 id
name    名称，一般也是唯一的
style    规定元素的行内样式（inline style）
title    规定元素的额外信息（可在工具提示中显示）
...

```

> 注意：实际中很少用到，都通过css和js来设置！

#### **注释**

```html
//注释:<!--注释-->
<a href="www.baidu.com">百度一下 你不知道</a> <!--注释写在这里-->

//注释一行代码
<!-- 此刻不显示图片：
[站外图片上传中……(3)]
-->

//条件注释
<!--[if IE 8]>
    .... some HTML here ....
<![endif]-->
```

## **㈢ 元素(标签+属性+文本)**

#### **HTML 元素：**

HTML 元素指的是从开始标签（start tag）到结束标签（end tag）的所有代码。

* HTML 元素以开始标签起始
* HTML 元素以结束标签终止
* 元素的内容是开始标签与结束标签之间的内容;某些 HTML 元素具有空内容（empty content）
* 大多数 HTML 元素可以嵌套。


### **1.文字**

```html
// 文本格式化，一些常用于设置文本字体的元素：
<b>字体加粗</b>
<i>斜体字体</i>
<u>下划线</u>
<s>删除线</s>

上标：X<sup>2</sup>
下标：Y<sub>3</sub>

//字体相关属性：
<font size="5" color="red" face="黑体">字体，添加属性值</font>  
<font size="3" color="#333333" face="黑体">size的值是1~7；color的表达方式：英语单词 RGB 十六进制</font>
```


### **2. 标题 段落 换行 水平线**

```html

// 标题。标题有六种大小h后的数字越大，说明标题越大。分别为

<h1 align="center">1号标题</h1>
<h2>2号标题</h2>
<h3>3号标题</h3>
<h4>4号标题</h4>
<h5>5号标题</h5>
<h6>6号标题</h6>


//段落：<p></p>
// 在定义了段落后，可以利用属性align来对段落进行设置。属性align的值包括left（左对齐）、center（居中对齐）、right（右对齐）
<p>第一段</p>
<p align="left">第二段</p>
<p align="center">第三段</p>
<p align="right">第四段</p>


//换行符 ：<br />                 
<br />  //换行


//水平线:<hr />
<hr />
<hr size="10" width="800"/>
<hr size="10" width="800" noshade="noshade"/>  
<hr size="30%" width="80%" /> //随屏幕百分比变化
```

### **3. 图片 超链接 锚点链接**

```html
/* 相对路径和绝对路径
 绝对路径：协议+主机+路径+文档
 相对路径：./ 当前目录  ../ 父级目录   / 根目录   ../../父目录的父目录

URL：scheme://host.domain:port/path/filename
*/

//图像:<img src="" />


属性：
scr    //source 图像的URL地址
title  //鼠标悬停显示的图片描述
alt    //在浏览器无法载入图像时展示给读者提示的信息
width
height
broder //边框


// 超链接：<a href=""></a>
// a标签用来定义一条超链接，其中要有的是href属性，href的作用是指明超链接要链接到的网址。除了href属性，还有title属性表示链接的提示信息。target属性表示链接的打开方式，即当点击了链接，选择是在另一个页面打开还是本页面打开。其属性值包括_blank(新的空白页)、_self(当前页)，_top（当前页）。

<a href="#" target="_blank">百度一下</a> 

// href的值可以是外部链接，也可以是内部文件，如***.html文件。

<a href=“http://www.163.com”>外部链接</a>

<a href=“about.html”>内部链接 </a>

// href也可以链接到别的地址，如邮箱、电话、sms。

<a href=“1233456.qqcom”>邮件链接</a>

<a href=“tel:电话号码”>拨打电话</a>

<a href="sms:139xxxxxxx">发送短信</a>


// href: 链接地址
// target: 定义被链接的文档在何处显示  _blank(新标签打开)  
                                _self (当前标签打开) 
                                _parent
                                _top


// 有时我们在浏览网页时会发现，有些网页比较人性化，会有点击返回顶部的按键。这样的效果其实用锚点标签就能做到。锚点就是点击使用户跳到文档的某个部分。
<a href="#位置名"> </a>

<a name="位置名"> </a> 

如代码例子：
<a href="#map">跳转</a>
<p id="map">代码代码</p>


```

### **4. HTML的实体**

```html
在 HTML 中，某些字符是预留的：小于号（<）和 大于号（>），会误认为是标签。
因此，在 HTML 源代码中使用字符实体（character entities）来显示预留字符。
&nbsp;  //空格
&quto;  //引号
&yen;  //￥
&times; 
&divede;
```

![HTML的实体](http://img.blog.csdn.net/20171109201331476?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvTWFjXzc2OQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)




### **5. 列表: ol ul li**

```html
分为：
   有序列表:<ol></ol> 
   & 
   无序列表:<ul></ul>

1）有序列表： 用于显示具有统一特征的有序数据

<ol type="i" start="3">
  <li>新闻1</li>
  <li>新闻2</li>
  <li>新闻3</li>
  <li>新闻4</li>
</ol>

属性   值              描述
type   1 数字(默认)    排序
       a 字母
       A 大写字母A
       i 小写罗马
       I 大写罗马
start  数字           起始数字


2）无序列表：用于显示同一特征的无限数据

<ul type="circle">
  <li>...</li>
  <li>...</li>
  <li>...</li>
</ul>

属性   值                  
type   disc 实心圆(默认)     
       circle  空心圆
       square 实心矩形
       none  无


3）定义列表：用来组织术语和它们的定义。任何信息如果包含多个术语和相对应的解释，都可以使用定义列表进行组织。
<dl>
	<dt>...</dt>
	<dd>...</dd>
	<dt>...</dt>
	<dd>...</dd>
</dl>


```

### **6. 表格: table**

* 用途：table元素的作用是显示表格化的数据！

* table元素可以嵌套。

```html
//用途：table元素的作用是显示表格化的数据！

<table>  ---------表格
  <tr>   ---------行
    <th>内容</th>  ---------单元格(字体加粗)
    <td>内容</td>  ---------单元格
    <td>内容</td>
  </tr>
</table>


table属性               值           
width
height
bgcolor           背景颜色（英语颜色；RGB；十六进制）
background        背景图片
border
bordercolor
cellpadding       单元格与内容之间的间距
cellspacing       单元格与单元格的边距
align  


tr属性            值
align           (left|center|right)
bgcolor         (英文颜色|rgb（255，255，255）|十六进制)
valign          垂直对齐方式（top|middle|bottom）



th td属性         值
align           (left|center|right)
bgcolor         (英文颜色|rgb（255，255，255）|十六进制)
valign          垂直对齐方式（top|middle|bottom）
rowspan         行合并
clospan         列合并



<table border="1" bordercolor="red" cellpadding="0" cellspacing="0" bgcolor="pink" align="center">
  <tr>
    <th colspan="3">表格的表头：合并3列</th>
    <td rowspan="5">合并5行</td>
  </tr>
  <tr bgcolor="blank" align="left" valign="top">
    <th></th>
    <th></th>
    <th></th>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</table>




//表格的嵌套
<table border="1" cellspacing="0" cellpadding="10">
  <tr>
    <th>[站外图片上传中……(5)]</th>
    <td align="center" valign="top">
      <table>
        <tr>
          <th rowspan="6">JEEP 牧马人</th>
        </tr>
        <tr>
          <td>姓名</td>
          <td>CwLife</td>
        </tr>
        <tr>
          <td></td>
          <td></td>
        </tr>
        <tr>
          <td></td>
          <td></td>
        </tr>
         <tr>
          <td></td>
          <td></td>
        </tr>
        <tr>
          <td></td>
          <td></td>
        </tr>
        <tr>
          <td></td>
          <td></td>
        </tr>
      </table>
    </th>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
</table>
```

###**7. 表单: form**

* 作用：用于收集用户输入;

* 表单元素:

	<input type=""/> 根据不同的 type 属性，可以变化为多种形态。
	<select></select> 定义下拉列表。
	<textarea></textarea> 定义多行输入字段（文本域）。
	<button></button> 定义可点击的按钮。

```html
作用：用于收集用户输入;
表单元素: 指的是不同类型的 input 元素、复选框、单选按钮、提交按钮等等

<form action="action_page.php" method="POST" name="">
  表单元素...
</form>

属性
name      表单的名字
method    规定在提交表单时所用的方法：get/post
action    定义在提交表单时执行的动作




常用的表单元素:

<input type=""/>  根据不同的 type 属性，可以变化为多种形态。
<select></select>  定义下拉列表。
<textarea></textarea>  定义多行输入字段（文本域）。
<button></button> 定义可点击的按钮。

文本框：<input type="text"> 定义供文本输入的单行输入字段。
<input type="text" name="控件名字" value="值" maxlength="最大输入字符长度" size="控件宽度" readonly="readonly"（只读） />

密码框：<input type="password"> 定义密码字段。
<input type="password" name="控件名字" value="值" maxlength="最大输入字符长度" size="控件宽度" readonly="readonly"（只读） />

多选勾选控件：<input type="checkbox"> 定义复选框
<input type="checkbox" name="控件名字" value="值" checked="checked"(已选中) disabled = "disabled"(禁用控件) />

单选勾选控件：<input type="radio"> 定义单选按钮。
<input type="radio" name="控件名字" value="值" checked="checked"(已选中) disabled = "disabled"(禁用控件) />

提交表单按钮：<input type="submit"> 定义提交表单数据至表单处理程序的按钮。
<input type="submit" value="按钮字样" />

重置表单按钮：
<input type="reset" value="按钮字样" />

上传文件按钮：
<input type="file" name="文件名称">

隐藏域:
<input type="hidden" name="控件名字" value="值" />

按钮：<input type="button> 定义按钮。
<input type="button" onclick="alert('Hello World!')" value="Click Me!">

<!--
HTML5 增加了多个新的输入类型：（老式浏览器不支持的输入类型，会被视为输入类型 text）  
    •    color
    •    date
    •    datetime
    •    datetime-local
    •    email
    •    month
    •    number
    •    range
    •    search
    •    tel
    •    time
    •    url
    •    week

<input type="number"> 用于应该包含数字值的输入字段。
<input type="number" name="quantity" min="1" max="5">

<input type="color"> 用于应该包含颜色的输入字段。
<input type="color" name="favcolor">

<input type="range"> 用于应该包含一定范围内的值的输入字段。
<input type="range" name="points" min="0" max="10">

<input type="date"> 用于应该包含日期的输入字段。
<input type="date" name="bday" max="1979-12-31"><br>

<input type="month"> 允许用户选择月份和年份。
<input type="month" name="bdaymonth">

<input type="week"> 允许用户选择周和年。
 <input type="week" name="week_year">

<input type="time"> 允许用户选择时间（无时区）。
<input type="time" name="usr_time">

<input type="datetime"> 允许用户选择日期和时间（有时区）。
<input type="datetime" name="bdaytime">

<input type="datetime-local"> 允许用户选择日期和时间（无时区）。
<input type="datetime-local" name="bdaytime">

<input type="email"> 用于应该包含电子邮件地址的输入字段。
<input type="email" name="email">

<input type="search"> 用于搜索字段（搜索字段的表现类似常规文本字段）。
<input type="search" name="googlesearch">

<input type="tel"> 用于应该包含电话号码的输入字段。
<input type="tel" name="usrtel">

<input type="url"> 用于应该包含 URL 地址的输入字段。
<input type="url" name="homepage">
-->



多行文本控件：
<textarea name="控件名称" cols="设置长度" rows="设置宽度">
  文本内容
</textarea>


下拉框控件：
<select name="控件名字">
  <option value="值" selected="selected"(已选中)>选择内容</option>
  <option value="值" >选择内容</option>
  <option value="值" >选择内容</option>
</select>

下拉选项的分组：
<optgroup label="分组标签01">
  <option value="值" selected="selected"(已选中)>选择内容</option>
  <option value="值" >选择内容</option>
  <option value="值" >选择内容</option>
</optgroup>


//e.g.
  <select name="请选择">
    <optgroup label="分组一">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
    <optgroup label="分组二">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
    <optgroup label="分组三">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
  </select>



按钮：
<button type="button" onclick="alert('Hello World!')">Click Me!</button>



实例：

<form name="" method="" action="">
  用户名：<input type="text" name="控件名字" value="" maxlength="" size="" readonly="readonly" />
  <br />
  密 码：<input type="password" name="控件名字" value="" maxlength="6" />
  <hr />
  多选一<input type="checkbox" name="控件名字" value="值" />
  多选二<input type="checkbox" name="控件名字" value="值" />
  多选三<input type="checkbox" name="控件名字" value="值" />

  <hr />
  男<input type="radio" name="控件名字" value="值" checked="checked" /> <!--默认选项；-->
  女<input type="radio" name="控件名字" value="值" /> <!--关联要同名字-->
  <hr/>
  <select name="请选择">
    <optgroup label="分组一">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
    <optgroup label="分组二">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
    <optgroup label="分组三">
      <option value="值" selected="selected">选择内容1</option> <!--默认选中-->
      <option value="值" >选择内容2</option>
      <option value="值" >选择内容3</option>
    </optgroup>
  </select>

  <hr/>
  <input type="submit" value="登录" />
  <input type="reset" value="重置按钮" />
  <button>按钮标题</button>

  <hr />
  <input type="file" name="filename">

</form>

```

### 8 图像热区 

&lt;area&gt;标记主要用于图像地图，通过该标记可以在图像地图中设定作用区域（又称为热点），这样当用户的鼠标移到指定的作用区域点击时，会自动链接到预先设定好的页面。其基本语法结构如下：
```html
   <area 
     class=type 
     id＝Value  
     href＝url  
     alt＝text  
     shape＝area-shape  
     coods＝value> 

```
shape和coords：是两个主要的参数，用于设定热点的形状和大小。其基本用法如下：

 * &lt;area shape="rect" coords="x1, y1,x2,y2" href=url&gt;表示设定热点的形状为矩形，左上角顶点坐标为（X1,y1），右下角顶点坐标为（X2,y2）。
 * &lt;area shape="circle" coords="x1, y1,r" href=url&gt;表示设定热点的形状为圆形，圆心坐标为（X1,y1），半径为r。
 *  &lt;area shape="poligon" coords="x1, y1,x2,y2 ......" href=url&gt;表示设定热点的形状为多边形，各顶点坐标依次为（X1,y1）、（X2,y2）、（x3,y3） ......。


&lt;area&gt;标记是在图像地图中划分作用区域的，因此其划分的作用区域必须在图像地图的区域内，所以在用 &lt;area&gt; 标记划分区域前必须用HTML的另一个标记&lt;map&gt;来设定图像地图的作用区域，并为指定的图像地图设定名称，该标记的用法很简单，即&lt;map name="图像地图名称"&gt; ...... </map&gt;。

HTML &lt;area&gt; 标签格式：
&lt;map&gt;&lt;area /&gt;&lt;/map&gt;

(这个标签的作用就是在一张图片中的某一特定位置定义一个(或多个)热点可进行超链接)
手动添加一个热点：选中一个图片/属性/选择一种形状如：矩形、圆形、多边形等。

**定义和用法**

<area> 标签定义图像映射中的区域（注：图像映射指得是带有可点击区域的图像）。

	area 元素总是嵌套在 <map> 标签中。

> 注释：<img> 标签中的 usemap 属性与 map 元素 name 属性相关联，创建图像与映射之间的联系。


【实例】：

带有可点击区域的图像映射：
```html
<img src="planets.jpg" border="0" usemap="#planetmap" alt="Planets" />
<map name="planetmap" id="planetmap">
  <area shape="circle" coords="180,139,14" href ="venus.html" alt="Venus" />
  <area shape="circle" coords="129,161,10" href ="mercur.html" alt="Mercury" />
  <area shape="rect" coords="0,0,110,260" href ="sun.html" alt="Sun" />
</map>
```
HTML 与 XHTML 之间的差异
在 HTML 中，<area> **没有结束标签**。
在 XHTML 中，<area> **必须正确地关闭**。

**提示和注释：**

>注释：<img> 中的 usemap 属性可引用 <map> 中的 id 或 name 属性（由浏览器决定），所以我们需要同时向 <map> 添加 id 和 name 两个属性



### **9 样式和脚本**

```html
//样式标签：<style></style>  
//脚本标签：<script></script>

```


### **10. 块: div span**

HTML 元素被定义为块级元素或内联元素。

* 块级元素：以新行来显示。
* 内联元素：不会以新行来显示。
```html
//div和span标签

<div> 元素是块级元素，常用于组合其他 HTML 元素的容器，进行文档布局。---
<span> 元素是内联元素，常用作文本的容器。


块级元素：
<body></body>
<div></div>  //常用的布局元素
<h1></h1>...<h6></h6>
<ol></ol>
<ul></ul>
<li></li>
<p></p>
<table></table>
<tr></tr>
<td></td>


内联元素：
<a href=""></a>
<i></i>
<u></u>
<b></b>
<span></span>  //文本标签
<font></font>
```
