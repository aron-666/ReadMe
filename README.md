#ReadMe
描述一个项目，一般都是通过README文件来编写。那么README文件是什么？
文件后缀md是markdown的缩写，markdown是一种编辑博客的语言。
不过GitHub支持的语法在标准markdown语法的基础上做了修改，称为Github Flavored Markdown。
最近对它颇感兴趣，便花了点时间研究下，整理出来，帮助大家快速了解README文件如何编写。

##关于标题
标题分为六个等级，等同于HTML h1 - h6，显示的文本大小依次减小。
不同等级之间是以井号#的个数来标识的。一级标题有一个#，二级标题有两个#，以此类推。

	#一级标题
	##二级标题
	###三级标题
	####四级标题
	#####五级标题
	######六级标题

注意井号#和标题名称要并排写作一行，效果如下：

#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题
######六级标题

================================

一、二级标题自带下横线，并且还有另外一种写法，比如：

	一级标题
	=========
	// 在文本下面加上等于号 = ，那么上方的文本就变成了一级标题。等于号的个数无限制，但一定要大于0。
	
	一级标题
	---------
	// 在文本下面加上下划线 - ，那么上方的文本就变成了二级标题，同样的，下划线个数无限制。
	
	注意：
	如果你只输入了等于号 = ，但其上方无文字，那么就只会显示一条直线。
	如果上方有了文字，但你又只想显示一条横线，而不想把上方的文字转义成大标题的话，
	那么你就要在等于号 = 和文字之间直接补一个空行。

##关于横线
要显示直线，符合显示横线条件的符号必须写三个以上，且其上方必须无文字。比如：

	=== 显示效果如下

===

	--- 显示效果如下

---

	*** 显示效果如下

***

	___ 显示效果如下

___

##显示文本
####普通文本
这是一段普通的文本

####普通文本换行
直接回车不能换行<br />
可以使用\<br>  
也可以在上一行文本后面补两个空格

或者就是在两行文本直接加一个空行，就像这样。

####单行文本
使用一个Tab实现单行文本，效果如下：

	Hello, Hanl.

####多行文本
多行文本和单行文本异曲同工，只要在每行行首加一个Tab，效果如下：

	Hello, Hanl.
	Hello, world.
	Hello, boy.

####部分文字高亮
如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，那么可以把它用 \`  \` 包围起来。
注意这不是单引号，而是Tab上方，数字1左边的按键（注意使用英文输入法）。比如：

	Hello, `Hanl`. what is your `phonenumber ?` // 效果如下

Hello, `Hanl`. what is your `phonenumber ?`

####删除线
想要实现文字删除线，可以把它用 \~~ \~~ 包围起来（注意使用英文输入法）。比如：

	这是一个 ~~删除线~~ // 效果如下

这是一个 ~~删除线~~

####斜体
想要实现文字斜体，可以把它用 \* \* 包围起来。比如：
	
	*斜体* // 效果如下

*斜体*

##关于链接
给一段文字加入链接的格式是这样的 \[要显示的文字\]\(链接的地址 提示文字\)。  
如果要引用的文件不存在，则待点击的文本为红色。引用的文件存在，则文本为蓝色。

####外部链接
	
	[百度](http://www.baidu.com "鼠标悬停显示") // 效果如下:

[百度](http://www.baidu.com "鼠标悬停显示") 

####外部链接另一种写法

	[百度][id]
	[id]:http://www.baidu.com "鼠标悬停显示" // 效果如下:

[百度][id]
[id]:http://www.baidu.com "鼠标悬停显示"

####本仓库内部链接

	[test](./test) // 效果如下:

[test](./test)

####锚点

	目标位置放<a name="xxx"/>
	设置锚点：[回到xxx](#xxx) 

[回到xxx](#xxx)

##显示图片
####外部链接的图片

	![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo") // 效果如下:

![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo")

####加上链接的图片

	[![head]](http://www.baidu.com/)
	[head]:http://www.baidu.com/img/bdlogo.gif "点击图片进入百度" // 效果如下:

[![head]](http://www.baidu.com/)
[head]:http://www.baidu.com/img/bdlogo.gif "点击图片进入百度"

##关于列表
####圆点列表

	* 昵称：Hanl
	* 年龄：24岁
	* 技能：html、css、javascript // 效果如下:

* 昵称：Hanl
* 年龄：24岁
* 技能：html、css、javascript

####数字列表

	1. html
	2. css
	3. javascript // 效果如下:

1. html
2. css
3. javascript

####数字列表自动排序

	1. html
	*  css
	*  javascript // 效果如下:

1. html
*  css
*  javascript

####复选框列表
	- [x] html
	- [x] css
	- [x] javascript
	- [x] php
	- [x] Android
	- [ ] swift
	- [ ] object-c // 效果如下:

- [x] html
- [x] css
- [x] javascript
- [x] php
- [x] Android
- [ ] swift
- [ ] object-c

####块引用
	
	>html
	>>css
	>>>javascript
	>>>>php // 效果如下:

>html
>>css
>>>javascript
>>>>php

##代码高亮
我们需要在代码的上一行和下一行用 \`\`\` 标记。\`\`\` 不是三个单引号，而是数字1左边，Tab键上面的键。
要实现语法高亮那么只要在 \`\`\` 之后加上你的编程语言即可（忽略大小写）。c++语言可以写成c++也可以是cpp。比如：
	
	```html
	<div><p class="readme">README</p></div> // html 效果如下:
	```
	效果如下:

```html
<div><p class="readme">README</p></div> // html
```

	```css
	.readme{color: red;font-size: 16px;} // css 效果如下:
	```

```css
.readme{color: red;font-size: 16px;} // css
```

	```javascript
	document.documentElement.title = "README"; // javascipt 效果如下:
	```

```javascript
document.documentElement.title = "README"; // javascipt 效果如下:
```

##添加表情
输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如`:blush:`，可以显示:blush:。

具体每一个表情的符号码，可以查询[emoji](./emoji.md)