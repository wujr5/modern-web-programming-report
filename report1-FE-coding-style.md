# 周四班-第11到15组 前端编程代码风格

## 1 第一次作业总结
### 1.1 总体上
> 本周作业总体问题不大，有些同学在index.html上面下功夫比较多，这个不错。全部同学也基本实现了要求的功能，所以分数都比较高。有些同学有创新，实现了另外的功能。因此得到了加分。

![](http://ww1.sinaimg.cn/large/ed796d65gw1ex6a3lz5uoj21kw0uaao6.jpg)
![](http://ww2.sinaimg.cn/large/ed796d65gw1ex6ahlvpaxj21kw0ub1kx.jpg)

### 1.2 存在问题
> 效果上，基本没问题。代码上，最大的问题就是HTML和CSS风格，还有CSS代码的冗余。
槽点如下。

#### 1.2.1 HTML缩进糟糕
![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6ajrs8kbj21b411s1dn.jpg)

#### 1.2.2 CSS缩进糟糕
![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6akhzpn3j217i11w13e.jpg)

#### 1.2.3 CSS代码冗余
![](http://ww2.sinaimg.cn/large/ed796d65gw1ex6alei70qj218213217k.jpg)

### 1.3 文件命名
> 文件命名是最大的槽点23333，知不知道TA每下一个文件夹都要修改你们的文件名，目前MA还没有提供全部下载的功能，所以一个一个下载非常痛苦([痛苦状表情])。

> 再补充一点是，一定要按照规定的命名格式来命名。否则扣分！

![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6apyid3kj20i80wkjwk.jpg)

吐槽完了，下面说一下web前端编程的代码风格的问题

## 2 HTML代码风格

先上一份代码风格良好的代码让大家感受一下。

![](http://ww2.sinaimg.cn/large/ed796d65gw1ex6b7l8wooj21ae11yh3f.jpg)
![](http://ww3.sinaimg.cn/large/ed796d65gw1ex6b8cywivj21ag122h3f.jpg)
![](http://ww2.sinaimg.cn/large/ed796d65gw1ex6b9np5f5j21be0u449c.jpg)
![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6b9zwh8yj21bk12k7if.jpg)

有没有感觉到赏心悦目！对！可读性良好的代码，看起来就是倍儿爽！

那怎样的代码才是可读性良好的代码呢？HTML究竟有什么样的编程风格？

### 2.1 高质量HTML

#### 2.1.1 从缩进开始说起

> 写HTML代码一定要注意缩进，在同一层次的代码就有相同的缩进，比如上面的风格良好的示例代码。`<head>`和`<body>`是具有相同的层次的，因此他们的缩进相同，`<html>`在最外层，所在的层次最低，因此没有缩进。其他的一样的道理。

> 除了缩进就是空行和注释了。我们可以根据语义或者结构，利用空行，把代码划分成多块。空行还可以放一些注释，用来说明你这段程序的作用。

#### 2.1.2 语义化标签

* 了解HTML标签的全称
![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6hlowgmaj21hq214tmx.jpg)

> 参考链接: [HTML常用标签及其全称][]

[HTML常用标签及其全称]: http://www.cnblogs.com/debuging/archive/2011/10/19/2217337.html

> 我们要了解所有标签所表达的含义。一般来说标签都是有语义的，比如`<p>`表示段落，`<div>`表示分割，等等。我们要根据标签设计出来是为了表达什么的，还有能表达什么，或者用在什么场合，进而决定选择什么标签。而不是都用`<div>`或者都用`<p>`。

* 少使用样式标签
> 所谓样式标签其实就是，具有浏览器默认样式的标签，比如`<strong></strong>`，`<bold>`，`<em>`等，让HTML回归表示结构，让CSS完全控制样式。做到结构和样式的分离。

* 根据内容将代码分不同的模块
> 也就是上面说的，利用空行和注释分割代码。把具有类似结构或者表达内容的代码划分到一个模块当中，比如一个`<div>`，然后使用相应的`class`或者`id`进行标识。还可以利用`<ul>`和`<li>`来进行内容块的划分。

* 判断网页语义是否良好
> 当一个网页完全去除CSS的时候，就可以观察其HTML结构，这时就能看到网页HTML结构是否良好。举例如下：

我们先来看一张图片，这时[w3c]官网的截图。

![](http://ww3.sinaimg.cn/large/ed796d65gw1ex6jvf8e57j21kw2l9b29.jpg)

[w3c]: http://www.w3c.org

下面是把网页去掉后的情况：

![](http://ww3.sinaimg.cn/large/ed796d65gw1ex6jxv0uy6j21kw6wsnpe.jpg)

大家可以看到两张图的对比。当没有样式，仍然不影响我们读取其中的内容，网页结构非常良好。这就是判定结构是否良好的标准。比较主观，关键在于看，去掉css后，html文件可读性是否良好。


## 3 CSS代码风格

### 3.1 糟糕的CSS

* 命名不友好，`class`和`id`，的命名乱七八糟，无意义
* 缩进问题，糟糕的缩进，代码成团，结在一起
* 代码冗余，每个地方都有相同的属性值

### 3.1 高质量的CSS

* `class`和`id`根据语义命名，有表达的意思，让人一看就懂。命名不怕长，就怕表达意思不清晰。
* `class`和`id`与大括号之间应该保留一个空格，属性应该有一个缩进，比如：
   ![](http://ww4.sinaimg.cn/large/ed796d65gw1ex6kas0i0tj20rw06amxz.jpg)

>   顺便举一个css风格良好的例子：

>   ![](http://ww2.sinaimg.cn/large/ed796d65gw1ex6kgeb3lyj21d80xsk30.jpg)

>   ![](http://ww1.sinaimg.cn/large/ed796d65gw1ex6kgs424cj21d60kw0ya.jpg)

* 代码精简。如果多个`class`或者其他标签具有相同的css属性的时候，就应该考虑把相同部分的内容抽取出来，独立成一个`class`

* css属性的排序。一个`class`或者`id`、标签里面的css属性应该按照什么顺序排列呢？这里有多重参考方案。
	> 比如：

	> 1. 按照字母序排列属性 

	> 2. 按照实现功能的相似性，比如处理字体的放在一块，然后空行，然后是处理图片的属性 

	> 3. 按照添加日期，也就是你先后添加的顺序来排列属性。
	
	> 初学者一般用的是第三种方案，但是并不建	议使用。最建议使用的是第二点，看起来非常清楚。其次是第一点，优点是能快速定位属性。
	
	> 希望同学们意识到这一点，从而改善自己的代码。
