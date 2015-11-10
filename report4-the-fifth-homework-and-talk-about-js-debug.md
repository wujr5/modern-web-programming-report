# 周四班-第16到第20组 问题总结和谈谈js调试

## 1 问题总结

### 1.1 html嵌入js函数

违反`结构、样式、行为`分离的原则。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2bbsin2j21320mo7mz.jpg)

### 1.2 css选择器全是id，属性冗余

css选择器过多使用id导致属性冗余。

![](http://ww3.sinaimg.cn/large/ed796d65gw1exw2buva08j20ho0qywko.jpg)

### 1.3 html使用表格布局

表格应该用来呈现数据，而不应该用来布局，布局任务应该有css承担。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2cwip7xj20to0y0qf5.jpg)

### 1.4 js函数臃肿

js函数非常庞大。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2e11y2ej21kw11dgyp.jpg)

### 1.5 尴尬的全局变量

全局变量滥用，污染全局空间。

![](http://ww3.sinaimg.cn/large/ed796d65gw1exw2hamdt5j20vs0teq93.jpg)

## 2 优点

### 2.1 界面做的很用心。

![](http://ww4.sinaimg.cn/large/ed796d65gw1exw2kaxxy4j20sa0y240b.jpg)

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2kkxpusj20p60n0ad2.jpg)

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw2kwopqsj20n40pwdi4.jpg)

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2l81vh2j20xw0tednb.jpg)

### 2.2 使用try catch捕获错误

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw2nfgntmj20yk0esn1s.jpg)

## 3 谈谈js调试

> 写任何一门语言的代码，都不可能一蹴而就，js也一样。涉及到逻辑处理的代码，出现错误，或者代码行为不符合预期的时候，最重要的就是快速定位错误，搞清楚出问题的原因。这个过程就是调试的过程。

> 以下我就我的经验，谈谈在浏览器控制台，js的调试技巧。

### 3.1 认识浏览器控制台

#### 3.1.1 概览

六个功能区：Elements，Network，Sources，Timeline，Profiles，Audits，Console

![](http://ww4.sinaimg.cn/large/ed796d65gw1exw39f68r5j21ew1201kx.jpg)

#### 3.1.2 Elements

这个功能区，最大的功能莫过于查看html，还有对应元素的css了。html的内容同学们很熟悉了。关键是css的查看，可能还需要了解多一些。比如下面。

**Styles** 

查看某元素详细的css，包括继承，默认的，还有自己的。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw3kg6l1mj21ey1224ne.jpg)

**Computed**

查看元素盒模型，可以实时改变width，height，border，padding，margin的值。

下面还可以看到属于元素自己的css属性值。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw3o4aoehj21f0122qrb.jpg)

**Event Listeners**

在元素上绑定的事件监听器。这个我不常用，不熟悉，如有见解，望不吝评论。

![](http://ww4.sinaimg.cn/large/ed796d65gw1exw3w6edwpj21eu1207sa.jpg)

**DOM Breakpoints**

在该元素对应的DOM元素所涉及的断点。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw43uhc5sj21eu128qoj.jpg)

**Properties**

该元素涉及的各种属性。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw459jizsj21ey124kd4.jpg)

#### 3.1.3 Network

网络监控区。监控在网页范围内的各种资源请求。不过这个需要在打开控制台之后，重新刷新网页才能收集到相关信息。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw5xxsomzj21fy12049t.jpg)

点开其中一个资源查看详情，可以看到各种相关信息。

![](http://ww4.sinaimg.cn/large/ed796d65gw1exw5z9f6qmj21fy1207ce.jpg)

#### 3.1.4 Sources

源文件区。在这里可以集中看到网页引用或者设计的，js，html，css文件。这个区域非常重要，用来进行js调试。下面在调试技巧那里具体说明。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw6fc04sij21g01247ky.jpg)

#### 3.1.5 Timeline

时间线。资源请求的详细时间情况。这个也是需要重新刷新网页才能收集到相关信息。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw6dl1rrbj21fy124dt8.jpg)

#### 3.1.6 Profiles

profiles区域。用来检测js运行是内存和cpu的运行情况。应该是作性能研究之用，我很少用。如有见解，望不吝评论。

![](http://ww3.sinaimg.cn/large/ed796d65gw1exw6jgoxwpj21fy11y434.jpg)

#### 3.1.7 Resources

资源区。在这里可以随时查看该网页或者网站对应的，各种数据资源。比如：数据库信息，local storage的信息，session，cookies等。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw6lorwyzj21g011wdk8.jpg)

#### 3.1.8 Audits

审计区。用来审查网页加载性能，组成情况，等等。这里有很多浏览器对网页分析的信息，很有用。

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw6p4slq0j21fy11ydj9.jpg)

![](http://ww2.sinaimg.cn/large/ed796d65gw1exw6qob876j21fs122to3.jpg)

#### 3.1.9 Console

控制台。在这里可以查看js的`console.log`或者`console.dir`输出。或者查看一些错误，或者直接可以运行js语句。极其有用的区域。

#### 3.1.10 快捷键

在其他区域调出Console区。快捷键：`esc`。比如在elements区域，调出console功能区。再按一次`ese`键即可隐藏它。

![](http://ww3.sinaimg.cn/large/ed796d65gw1exw6ub6wzgj21g01241b7.jpg)

其他快捷键：点击菜单自行查看。

比较有用的有：`control + L`清楚console区域的信息。

![](http://ww1.sinaimg.cn/large/ed796d65gw1exw6wuwq0nj21g211ykci.jpg)

### 3.2 错误查看

在console区，会输出js运行时发生的错误，因此通过这些错误，我们就可以及时知道我们的程序出现了问题。然后根据信息，快速定位错误发生的位置。

比如：我现在故意讲程序中的一个函数名字改成另外的名字。刷新网页，点击一下出发该函数的按钮。然后控制台马上就输出了错误信息。

`sumUp is not defined`提示说`sumUp`不是一个函数。

我就可以根据这个信息，马上找到sumUp使用的地方，然后去查看js文件，看看为什么没有定义这个函数。最后发现是函数名不一致，然后马上就可以把程序修改正确。

![](http://ww4.sinaimg.cn/large/ed796d65gw1exw7526635j21ac120n0d.jpg)

### 3.3 输出调试

调试的时候，可以使用以下两个命令讲js运行时的变量数值，或者字面量输出到控制台。

就像是C语言中的`printf`，或者C++中的`cout`，或者java中的`System.out.println`

#### 3.3.1 console.log

最简单的方法是console.log()，可以用来取代alert()或document.write()。

#### 3.3.2 console.dir

console.dir()可以显示一个对象所有的属性和方法。

参考：(这个一定要看！)

[Firebug控制台详解][] 

[Firebug控制台详解]: http://www.ruanyifeng.com/blog/2011/03/firebug_console_tutorial.html

### 3.4 查看数值

### 3.5 断点调试

### 3.6 二分调试法
