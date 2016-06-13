# 简介(Introduction)
web浏览器应该是使用最广泛的软件了。在这里，我将要讲述下它们在幕后是怎么工作的。我们
来看一下从你在地址栏里输入“google.com”到谷歌的页面显示在浏览器窗口里都发生了什么。


## 我们要讨论的浏览器
> 　　目前使用的主流浏览器有五个：Internet Explorer、Firefox、Safari、Chrome 浏览器和 Opera。
> 本文中以开放源代码浏览器为例，即 Firefox、Chrome 浏览器和 Safari（部分开源）。根据 StatCounter 
> 浏览器统计数据，目前（2011 年 8 月）Firefox、Safari 和 Chrome 浏览器的总市场占有率将近 
> 60%。由此可见，如今开放源代码浏览器在浏览器市场中占据了非常坚实的部分。

> 现在有五款主要的浏览器：Internet Explorer、Firefox、Safari、 Chrome 和 Opera。
> 我会给出几个例子，它们来自于开源浏览器Firefox、chrome还有部分开源的safari。
> 根据W3C浏览器统计信息，当前（2009年10月），Firefox、 Safari和Chrome的市场占有率接近60%。
> 所以当前开源浏览器已经成为了浏览器行业的重要组成部分。


浏览器的历史就是互联网的历史，浏览器大战，chorome的崛起，兼容性问题，hack方式，HTML5和CSS3的支持性。
其实前端的所有问题都会浏览器的问题，如果一开始标准统一，就不会有后来的问题。但是浏览器后面的利益和势力太大了，毕竟这是一个时代的入口。是打开未来的那把钥匙。

不同的浏览器有不等同的内核，上面的五款浏览器是主流，至于360浏览器，搜狗浏览器都是中国特色，其内核和上面五款浏览器相近。
而且所有的浏览器都是有版本的问题，同一款浏览器的不同版本是不同的，不同就是内核的实现机制不同，这种不同会导致兼容新问题，而探究这种不同，让不同浏览器有相同的输出是我们需要达到的目的。



## 浏览器的主要功能
> 浏览器的主要功能是展现你所需要的web资源，它从服务器端请求资源并显示在浏览器窗口上，
> 资源格式一般为html,但是也可以是pdf，image或者其他的格式。资源的地址是由用户通过URI
> （统一资源定位符）来指定的，关于这个在网络那章里做更多的介绍。
> HTML和CSS规范里指定了浏览器解析和显示HTML文件的方式，W3C维护这些规范，它们是web的标准化组织。

> HTML的当前版本是4，第5版正在进行中。CSS的当前版本是2，第3版正在进行中。
> 过去的很多年里，各个浏览器都是只遵守规范的一部分，然后做它们自己的扩展，这对于web开
> 发者来说引起了严重的兼容性问题，现在浏览器大都或多或少的遵守了规范。
> 各浏览器的用户界面彼此有很多共同的地方，共同的元素有：
> 1.键入URI的地址栏
> 2.后退和前进按钮
> 3.书签菜单
> 4.用来刷新和停止当前文档加载的刷新和停止按钮
> 5.帮你返回主页的主页按钮

> 说来奇怪，并没有任何正式的规范指定浏览器的用户界面，这只是多年试验以及各浏览器互相模
> 仿形成的一个好的做法。HTML5规范中没有定义浏览器一定会有哪些UI元素，但是列举出了一
> 些通用的元素，有地址栏、状态栏和工具栏。当然，特定浏览器还有一些独一无二的特征，比如
> Firefox的下载管理。关于这个在UI那章里做更多的介绍。

浏览器就像是“我的电脑”，打开我的电脑可以查看和打开文件，浏览器的左右也是相似，只是在浏览器上面，文件的查找和查看都是在浏览器上面完成的。
浏览器就是一个全球的“我的电脑”，连接网络，就可以查看全世界的文件和资源。
在windos系统下面，浏览器和“我的电脑”的UI界面也是相似的。上面的浏览器的特性“我的电脑”也全部具备。
我以前一直认为页面是文档，是和word，excel相同的存在，只是这种文档是被放到网络上和人共享的，但是页面终究是逃不出文档的文类，有文档应当具有的特性。这点我们在HTML的标签中可以看出，可以发现其实word和页面是想通的。
所谓的HTML语义化也就是写一个标准的word文档，有严格的排版要求。
我认为写面页面就应该像写毕业论文一样，严格的按照格式要求来。
html中的doctype，p ，其他的语义化标签都在告诉我们，页面是一个文档，而不是一个程序。浏览器无非就是展现这个文档的软件，就像是office。
其实在这点上面来说写页面应该像office一样每个人应该掌握的技巧。这点可能在10年以后会发生。

## 浏览器的高级结构

> ### HTML5 Cavans

