MarkDown笔记
===========

段落和换行
----------

1. 一个以上的空格   
2. 两个以上的空格加换行

标题
----

1. 最高阶标题

    This is an H1   
    =============

2. 第二阶标题

	This is an H2   
	-------------

3. 1到6阶标题

	#This is an H1   
	##This is an H2   
	######This is an H6   

        闭合标题

	#This is an H1   
	###This is an H3###   

引用
----

1. 每行前面加上>   
2. 可嵌套

列表
----

1. 无序列表,每行前加*,+,-   
2. 有序列表,每行前加数字和点

程序代码块
----------

1. 缩进 4 个空格或是 1 个制表符   
2. 小段行内代码用反引号(`` ` ``)

分隔线
------

* 三个或以上的星号、减号

链接
----

1. 方括号后面马上接着圆括号并插入网址链接   

    This is [an example](http://example.com/ "Title") inline link.

2. 参考式的链接是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记

    This is [an example][id] reference-style link.
    [id]: http://example.com/  "Optional Title Here"

3. 隐式链接标记

    [Google][]
    [Google]: http://google.com/

强调
----
1. 斜体

    *italic* _italic_

2. 粗体

    **bold** __bold__

图片
----

* 一个惊叹号 !
* 接着一对方括号，里面放上图片的替代文字
* 接着一对普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 文字。

        ![Alt text](/path/to/img.jpg)


自动链接
-------

* 用尖括号包起来

        <http://example.com/>   
        <address@example.com>
