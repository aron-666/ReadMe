# ReadMe
描述一个项目，一般都是通过README文件来编写。那么README文件是什么？
文件后缀md是markdown的缩写，markdown是一种编辑博客的语言。
不过GitHub支持的语法在标准markdown语法的基础上做了修改，称为Github Flavored Markdown。
最近对它颇感兴趣，便在网上搜集并整理了一些资料，帮助大家快速了解README文件如何编写。

## 关于标题
标题分为六个等级，等同于HTML h1 - h6，显示的文本大小依次减小。
不同等级之间是以井号#的个数来标识的。一级标题有一个#，二级标题有两个#，以此类推。

	#一级标题
	##二级标题
	###三级标题
	####四级标题
	#####五级标题
	######六级标题

注意井号#和标题名称要并排写作一行，显示效果如下：

#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题
######六级标题

================================

一、二级标题自带下横线，并且还有另外一种写法，如下：

	一级标题
	=========
	// 在文本下面加上等于号 = ，那么上方的文本就变成了一级标题。等于号的个数无限制，但一定要大于0。
	
	一级标题
	---------
	// 在文本下面加上下划线 - ，那么上方的文本就变成了二级标题，同样的，下划线个数无限制。

	如果你只输入了等于号=，但其上方无文字，那么就只会显示一条直线。
	如果上方有了文字，但你又只想显示一条横线，而不想把上方的文字转义成大标题的话，
	那么你就要在等于号=和文字之间直接补一个空行。
