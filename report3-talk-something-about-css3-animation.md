# 周四班第三次作业总结 & life coding show & css3动画初探

## 1 第三次作业总结

### 1.1 优点

#### 1.1.1 开始有意识地添加注释

![](http://ww3.sinaimg.cn/large/ed796d65gw1exhm42f5j2j20ve13cjxo.jpg)
![](http://ww3.sinaimg.cn/large/ed796d65gw1exhm4jhg15j215o0ykn3f.jpg)
![](http://ww1.sinaimg.cn/large/ed796d65gw1exhm5wzm9cj20li0qw461.jpg)

#### 1.1.2 效果大致符合要求，都有自己用心的思考

![](http://ww1.sinaimg.cn/large/ed796d65gw1exhm7pifwpj20ow0iewfc.jpg)

#### 1.1.3 自己记录改进过程

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhm942x8gj20tc0jiac2.jpg)
![](http://ww1.sinaimg.cn/large/ed796d65gw1exhm9h2ssej20xu0yydoi.jpg)

#### 1.1.4 大部分同学的代码风格都不错

参考： [前端编程代码风格][]

[前端编程代码风格]: https://github.com/wujr5/modern-web-programming-report/issues/1

#### 1.1.5 大部分同学的作业都符合题目要求，小圈的散开收回、大圈和@的缩放都很完整，与视频效果吻合。

#### 1.1.6 有的同学的外观和设计图基本吻合，找不到任何瑕疵。

![](http://ww3.sinaimg.cn/large/ed796d65gw1exhmg0q4xrj20ob0i5ac6.jpg)

#### 1.1.7	有同学提供的github链接中，有markdown语法所写的readme

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhmi58tkfj21kw0p6dj7.jpg)

### 1.2 缺点

#### 1.2.1 效果理解有偏差

> 大气泡内容，缩放原点；小气泡缩放原点；中心气泡缩放原点；动画颤抖；

#### 1.2.2 css注释符号不清

> 注释有点让人看不太懂，可能适得其反。

#### 1.2.3 position属性特点不清

```
position: static, absolute, relative, fixed
```
> 参考：

> 1. [学习css布局][]
> 2. [MDN position][]

[学习css布局]: http://zh.learnlayout.com/position.html
[MDN position]: https://developer.mozilla.org/zh-CN/docs/Web/CSS/position

#### 1.2.4 作业的一些细节要求没有完成

> 配色，动画时间，大小等

#### 1.2.5 仍有相当部分同学没按要求命名

> 这个不多说

#### 1.2.6 有的同学注释写的太多了

> 如果能确定大家基本能看懂的地方，就不用注释啦。注意注释冗余。

#### 1.2.7 比较多同学没有仔细观察视频的动画效果：鼠标移开之后没有做到小圈先收回，@再缩小。

> 这是普遍存在的问题。

#### 1.2.8 部分同学的外观和设计图相差较大。

> 这个呵呵😷

![](http://ww3.sinaimg.cn/large/ed796d65gw1exhml27g1lj20oh0j1dhv.jpg)

### 1.3 优秀作业展示

#### 1.3.1 优秀作业

```js
14331291	吴思
14359047	洪生楠
14331077	关伟杰
14331091	胡南
14353101	黄炜
14331034	陈颂熙 
14331051	邓杰友
14331231	邱天睿
14331136	李为
14331327	颜鹏翔
14331020	陈纪庚
14331295    吴子昊
14331030    陈锐彬
14332011    梁权民
```

#### 1.3.2 优秀作业展示

![](http://img5.duitang.com/uploads/item/201404/21/20140421150445_8c5GQ.jpeg)
![](http://img4.duitang.com/uploads/item/201407/29/20140729171143_Gatjz.jpeg)

#### 1.3.3 郝思佳：作业提点

> 有请美女TA 😍

## 2 life coding show

### 2.1 王老师 coding show

😄 [王老师codingshow] 😄

[王老师codingshow]: http://static.youku.com/v1.0.0577/v/swf/loader.swf?VideoIDS=XMTM2ODkzNzkzNg%3D%3D&embedid=NDUuMTI0LjY0LjIzOQIzNDIyMzQ0ODQCbXkuc3Muc3lzdS5lZHUuY24CL3dpa2kvZGlzcGxheS9XRUIvVHV0b3JhaWwrMDEuK0hvdyt0bytzdHlsZSthK1JJQSt3ZWJwYWdl&wd=&vext=pid%3D%26emb%3DNDUuMTI0LjY0LjIzOQIzNDIyMzQ0ODQCbXkuc3Muc3lzdS5lZHUuY24CL3dpa2kvZGlzcGxheS9XRUIvVHV0b3JhaWwrMDEuK0hvdyt0bytzdHlsZSthK1JJQSt3ZWJwYWdl%26bc%3D%26type%3D0

新地址：[codingshow][]

[codingshow]: http://v.youku.com/v_show/id_XMTM3MzEyOTQ3Ng==.html

![](http://ww1.sinaimg.cn/large/ed796d65gw1exhttlbwqij21g80tyjxw.jpg)

## 3 css3动画初探

### 3.1 网页动画

总体来说有三种方式可以实现网页动画。

首先，是JavaScript实现。一般来说会直接使用JavaScript函数库，很少自己实现JS动画，因为比较复杂。优秀的函数库有`JQuery`等，还有一般的前端框架都会提供js动画。比如`Bootstrap`，`Materialize`等。

> 由于目前我们还没有学习JS的只是，这部分的内容不讲。

其次，是CSS3中的`transition`实现。`transition`翻译为过渡，意思是当一些CSS属性发生变化的时候，通过设置`transition`，可以控制变化的过程。因此我们能够利用过渡实现动画。

第三，是CSS中的`animation`实现。`animation`是3D变形，比transition更复杂，功能也更强大。

### 3.2 transition 过渡

过渡其实是对于某个属性，或者某些属性而言的。比如，

```html

<style>
	div {
		width: 100px;
		height: 100px;
		background: blue;
	}
	
	div:hover {
		width: 200px;
		height: 200px;
	}
</style>

<div></div>

```

当鼠标hover在div上的时候，div的宽度和高度就会突变成为200px，这时是突然变化的，没有过渡，也可以认为是动画，但是不美观。

`transition`属性就是用来调和这个变化过程的。

举个例子。[transition intro][]

[transition intro]: http://codepen.io/anon/pen/avGMpX

transition：[MDN transition][]

[MDN transition]: https://developer.mozilla.org/zh-CN/docs/Web/CSS/transition

transition语法：

```css
transition: transition-property transition-duration transition-timing-function transition-delay[, ...]
```

属性如下：

1. `transition-property`：需要过渡处理的属性
2. `transition-duration`：延续时间
3. `transition-timing-function`：属性值随时间的变化函数
4. `transition-delay`：执行动画的延迟时间

```css
transition-timing-function:

ease: 缓解效果，立方贝塞尔曲线
linear: 线性效果
ease-in: 渐显效果
ease-out: 渐隐效果
ease-in-out: 渐显渐隐效果
cubic-bezier: 特殊立方贝塞尔曲线
```

### 3.3 transform 2D变形

`transform`也可以看做是一个属性，包含很多变形函数。如果没有为`transform`设置`transition`，那也是一个瞬变效果，因此`transform`一般与`transition`配合使用。

举例说明。[transform example][]

[transform example]: http://codepen.io/wujiarong/pen/zvjXGY

transform函数：

```css
skew
matrix：矩阵变换
translate：移动元素
scale：缩放元素
rotate：旋转元素
skew：倾斜元素
```

### 3.4 animation 3D变形

举个例子：[animation 3d][]

[animation 3d]: http://codepen.io/wujiarong/pen/gazygv

animation语法：

```
animation: animation-name animation-duration animation-timming-function animation-delay animation-iteration-count animation-direction
```

```css
animation-name: 动画名称，对应关键帧的定义
animation-duration：动画时间
animation-timing-function：动画播放方式
animation-delay：延迟时间
animation-iteration-count：重复次数
animation-direction：播放方向
```
关键在于，定义关键帧。

```css
@keyframes keyframeName {
	0% {
		transform: rotateX(0deg);
	}
	50% {
		transform: rotateX(180deg);
	}
	100% {
		transform: rotateX(360deg);
	}
}
```

### 3.5 浏览器兼容处理

> 自己查阅相关资料。

## 4 本周作业

上周作业是正式分数。

本周作业不作为期末分数。只作为参考。

本周作业为，根据老师或者TA的提点，改进上周作业，按时提交。

改进原则：

```javascript
1. 更接近题目要求的效果
2. css代码可读性更好
3. 在第二点的基础上，css代码更短。DRY：don‘t repeat yourself
4. 改善你的代码风格
```

## 5 接下来安排

小组内互动交流讨论

## 6 Tool tips

> 老师视频上提到的开发工具，还有我自己推荐的开发工具

### 6.1 Sublime Text

相信这个大家已经有了。链接：[sublime text 3][]

[sublime text 3]:http://www.sublimetext.com/3

![](http://ww3.sinaimg.cn/large/ed796d65gw1exhxn0di7fj208w07cmx9.jpg)

### 6.2 Page Ruler

链接：[page ruler][]

[page ruler]: https://chrome.google.com/webstore/detail/page-ruler/jlpkojjdgbllmedoapgfodplfhcbnbpn

![](http://ww1.sinaimg.cn/large/ed796d65gw1exhxo6ivnqj21kw0ghdiz.jpg)

### 6.3 Colorzilla

链接：[Colorzilla][]

[Colorzilla]: https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxp09ilaj20cq0gq401.jpg)

### 6.4 Livereload

chrome插件结合软件一起使用。插件：[chrome livereload][]，桌面应用：[livereload][]

[livereload]: http://livereload.com/
[chrome livereload]: https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei

![](http://ww3.sinaimg.cn/large/ed796d65gw1exhxprsgvbj219o0x8n5r.jpg)

### 6.5 Markdown编辑器

三平台支持：[haroopad][]

[haroopad]: http://pad.haroopress.com/user.html#download

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxspfbm9j21kw0p9k2c.jpg)

Mac强烈推荐：[Mou][]

[Mou]: http://25.io/mou/

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxrudfyhj21e80yw7gj.jpg)


> 参考：

> 1. [Mac 下两款 Markdown 编辑器 Mou/MacDown 大 PK][]

> 2. [10款流行的Markdown编辑器，总有一款适合你][]

> 3. Markdown语法比较好的教程：[Garrett Flavored Markdown Reference Guide][]

[Garrett Flavored Markdown Reference Guide]: http://coapp.org/reference/garrett-flavored-markdown.html


[Mac 下两款 Markdown 编辑器 Mou/MacDown 大 PK]: http://www.jianshu.com/p/6c157af09e84
[10款流行的Markdown编辑器，总有一款适合你]: http://www.csdn.net/article/2014-05-05/2819623

### 6.5 微博图床

写Markdown文本时的利器，免费图片网盘。[新浪微博图床][]

[新浪微博图床]: https://chrome.google.com/webstore/detail/%E6%96%B0%E6%B5%AA%E5%BE%AE%E5%8D%9A%E5%9B%BE%E5%BA%8A/fdfdnfpdplfbbnemmmoklbfjbhecpnhf

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxeiyoxmj21d410gn00.jpg)

### 6.6 网页截图fireshot

可以全网页截图或者滚动截图：[fireshot][]

[fireshot]: https://chrome.google.com/webstore/detail/capture-webpage-screensho/mcbpblocgmgfnpjjppndjkmgjaogfceg

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxhlrfrcj20hs0a475m.jpg)

### 6.7 免费科学上网

这个我没有用过，大家不妨试下，同学推荐说好用。[lantern][]

[lantern]: https://github.com/getlantern/lantern

![](http://ww4.sinaimg.cn/large/ed796d65gw1exhxlwoqyxj216o0uy0xf.jpg)

### 6.8 去除页面牛皮癣

免费去除页面广告：[Adblock][]

[Adblock]: https://chrome.google.com/webstore/detail/gighmmpiobklfepjocnamgkkbiglidom

![](http://ww2.sinaimg.cn/large/ed796d65gw1exjhvc1k5oj21iw0ykws0.jpg)

