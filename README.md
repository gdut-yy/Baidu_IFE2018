# Baidu_IFE2018
百度前端技术学院2018学习笔记

## DAY 1 为什么有那么多人要做前端
关于笔记：

- 日期，今天的学习总用时，今天学习的目标是什么，是否达成
- 哪些东西今天了解得比较透彻，说说自己的理解
- 哪些东西今天了解到了一些，还有哪些点需要后续继续深入阅读
- 哪些东西今天学了之后还有很多疑问没有被解答，把问题记录下来，以待后续解决

立Flag，写下大家参加今年前端学院的目标，能不能和我们一起坚持66天！

codepen

## DAY 2 给自己做一个在线简历吧

	<h1>简历</h1>
	<h2>姓名:张三</h2>
	<h2>手机：18600000000</h2>
	<h2>邮箱：joinefe@baidu.com</h2>
	<h2>本科：百度前端学院</h2>
	<h2>项目A：</h2>
	<h3>项目时间：2017.1-2017.8</h3>
	<h3>项目描述：在项目A中负责了xxxxx</h3>

1、HTML是什么，HTML5是什么

- HTML 指的是超文本标记语言 (Hyper Text Markup Language)。
- HTML5是最新的HTML标准，拥有更丰富的语义、图形以及多媒体元素等内容。

2、HTML元素标签、属性都是什么概念？

- HTML不是编程语言，是标记语言，所以要使用标记标签来描述网页。
- 属性是用来提供HTML标签更多的信息。

3、文档类型是什么概念，起什么作用？

- 在互联网上有许多不同的文档，只有了解文档的类型，浏览器才能正确的显示文档。提前声明文档类型可以帮助浏览器正确的显示网页。

4、meta 标签都用来做什么的？

- 通常所说的META标签，是在 HTML 网页源代码中一个重要的 html 标签。META 标签用来描述一个HTML网页文档的属性，例如作者、日期和时间、网页描述、关键词、页面刷新等。

5、Web语义化是什么，是为了解决什么问题

- HTML的每个标签都有其特定含义(语义),Web语义化是指使用语义恰当的标签,使页面有良好的结构,页面元素有含义,能够让人和搜索引擎都容易理解。

6、链接是什么概念，对应什么标签？

- HTML \<a\> 元素 (或锚元素) 可以创建一个到其他网页、文件、同一页面内的位置、电子邮件地址或任何其他URL的超链接。

7、常用标签都有哪些，都适合用在什么场景

- body:在网页上要展示出来的页面内容一定要放在body标签中
- p:如果想在网页上显示文章，这时就需要p标签了，把文章的段落放到p标签中。标签的默认样式，段前段后都会有空白，如果不喜欢这个空白，可以用css样式来删除或改变它。
- span:标签是没有语义的，它的作用就是为了设置单独的样式用的。
- br:在需要加回车换行的地方加入br，br标签作用相当于word文档中的回车。在 html 代码中输入回车、空格都是没有作用的。在html文本中想输入回车换行，就必须输入br。没有HTML内容的标签就是空标签，空标签只需要写一个开始标签，这样的标签有br、hr和img。
- div:在网页制作过程过中，可以把一些独立的逻辑部分划分出来，放在一个div标签中，这个div标签的作用就相当于一个容器。什么是逻辑部分？它是页面上相互关联的一组元素。如网页中的独立的栏目版块，就是一个典型的逻辑部分。用id属性来为div提供唯一的名称，必须唯一。
- img:插入图片,img src=”图片地址” alt=”下载失败时的替换文本” title = “提示文本” src：标识图像的位置；alt：指定图像的描述性文本，当图像不可见时（下载不成功时），可看到该属性指定的文本；title：提供在图像可见时对图像的描述(鼠标滑过图片时显示的文本)；图像可以是GIF，PNG，JPEG格式的图像文件。


8、表单标签都有哪些，对应着什么功能，都有哪些属性

- form:可以把浏览者输入的数据传送到服务器端，这样服务器端程序就可以处理表单传过来的数据。form method=”传送方式” action=”服务器文件” . form标签是成对出现的，以form开始，以/form结束。action ：浏览者输入的数据被传送到的地方,比如一个PHP页面(save.php)。method ： 数据传送的方式（get/post）。所有表单控件（文本框、文本域、按钮、单选框、复选框等）都必须放在标签之间
- input:当用户要在表单中键入字母、数字等内容时，就会用到文本输入框。文本框也可以转化为密码输入框。input type=”text/password” - name=”名称” value=”文本” / 当type=”text”时，输入框为文本输入框;当type=”password”时, 输入框为密码输入框。name：为文本框命名，以备后台程序ASP 、PHP使用。value：为文本输入框设置默认值。(一般起到提示作用)
- textarea:当用户需要在表单中输入大段文字时，需要用到文本输入域。textarea rows=”行数” cols=”列数” 文本 /textarea rows ：多行输入域的行数。cols ：多行输入域的列数。在textarea /textarea 标签之间可以输入默认值。
- radio/checkbox:使用单选框、复选框，让用户选择,input type=”radio/checkbox” value=”值” name=”名称” checked=”checked”/> 当 type=”radio” 时，控件为单选框,当 type=”checkbox” 时，控件为复选框,value：提交数据到服务器的值（后台程序PHP使用）,name：为控件命名，以备后台程序 ASP、PHP 使用,checked：当设置 checked=”checked” 时，该选项被默认选中,同一组的单选按钮，name 取值一定要一致，这样同一组的单选按钮才可以起到单选的作用。
- submit:使用提交按钮，提交数据,input type=”submit” value=”提交”> type：只有当type值设置为submit时，按钮才有提交作用,value：按钮上显示的文字

9、ol, ul, li, dl, dd, dt等这些标签都适合用在什么地方，举个例子

- ol、ul、li适用无描述的列表。例如：新闻展示页面，一共N条新闻，点进去可浏览详情。
- dl、dd、dt适用有描述的列表 例如：简历页面，介绍自己的信息、年龄、住址等。


## DAY 3 让简历有点色彩

Mozilla 开发者社区（MDN）



## DAY 4 背景边框 列表 链接 和 更复杂的选择器

## DAY 5~6 三种简历

要求使用 resume.html 和 style_1.css、style_2.css、style_3.css 实现以下效果

![](resume1.png)

![](resume2.png)

![](resume3.png)

## DAY 7~8 学习布局