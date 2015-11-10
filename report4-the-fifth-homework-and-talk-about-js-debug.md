# 周四班-第16到第20组 问题总结和谈谈js调试

## 1 问题总结

### 1.1 html嵌入js函数

违反结构，样式，行为分离的原则。

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

![](http://ww3.sinaimg.cn/large/ed796d65gw1exw62eys2ij21fi11y4j7.jpg)

#### 3.1.5 Timeline

#### 3.1.6 Profiles

#### 3.1.7 Audits

#### 3.1.8 Console

#### 3.1.9 快捷键

### 3.2 错误查看

### 3.3 输出调试

### 3.4 查看数值

### 3.5 断点调试

### 3.6 二分调试法



