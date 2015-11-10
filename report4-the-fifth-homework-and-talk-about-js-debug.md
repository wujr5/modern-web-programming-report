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



### 3.2 错误查看

### 3.3 输出调试

### 3.4 查看数值

### 3.5 二分调试法



