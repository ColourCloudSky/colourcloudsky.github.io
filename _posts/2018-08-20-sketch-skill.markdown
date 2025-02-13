---
layout:     post
title:      "那些你可能没发现的Sketch冷知识【第一期】"
subtitle:   "Sketch use tips 【1】"
#date:       2018-08-20 16:35:00
author:     "Caiyunsky"
header-mask: 0.3
header-img: "img/article-img/20180820/post-bg-banner.jpg"
catalog:    true
tags:
    - sketch
---

> 全文共2992词，阅读大约需要10分钟

工作中发现，虽然仅使用基础功能也能很好的胜任设计工作，但是如果能掌握一些实用的小技巧则会让你的工作更加轻松。所以从本期开始，会陆续写一些关于sketch方面鲜为人知的小知识，可能会包括快捷操作，组件，库，实用插件等等，希望这系列的文章能抛砖引玉，对大家有所启发。

既然是冷知识，往往很难系统化的去梳理，可能会比较零散，所以大家看到感兴趣的小技巧最好去动手试下，应该就能很快明白了。

（注：每个人都有自己的使用习惯，套路，所以很难知道我写的对你来说是冷还是热。我只是把我自己从第一次使用sketch到现在的过程中，觉得是比较冷门但又很实用的小技巧分享出来。所以，学到了就点个赞，老司机们就请见谅吧~）

#### 1、在属性栏中快捷修改对象属性

平时大家在修改对象时，可以选择对象并直接进行缩放，其结果是往往容易出现偏差，比如小数像素，没有对齐等等，直接在右侧属性栏通过数值来操作会方便很多。

1）鼠标、Shift、Option实现快速修改

主界面中的右侧的属性栏中可以单击属性值以快速递增或递减该值（注意要把鼠标放在文字的上下方位内，出现左右箭头才可以快速修改）。如果按住Shift键，Sketch将相应地将值递增或递减10倍，按住Option键会将其增加/减少十分之一。

![1](/img/article-img/20180820/1.gif)

2)  属性栏还能支持组合修改

支持简单数学公式，支持样式单位L(中心点左对齐)R（中心点居右）C（中心点居中）M（中心点居中）T（中心点置顶）B（中心点底部对齐），支持圆角快速自定义(格式是X;Y;N;M，顺序是左上-右上-右下-左下)，能帮助快速精确调整，是不是很高级！？

![2](/img/article-img/20180820/2.gif)

数字+功能组合操作

![3](/img/article-img/20180820/3.gif)

简单数学公式计算

![4](/img/article-img/20180820/4.gif)

圆角快捷设置

#### 2、图层操作上的小技巧

在刚开始使用sketch时，经常会发生误操作，比如移错图层。比如你一开始选择到了某个图层，移动的时候还是把图层组给移动了，很头疼。所以在多图层堆叠时，有几个快捷键技巧挺实用。

1）当图层深埋在一堆文件夹中时，可以直接按住command+鼠标左键，可以快速选择组内的图层

![5](/img/article-img/20180820/5.gif)

2）按住Option，就会只选择完全位于某个图形区域内的图层，避免误选。（举个栗子，在一个有底部背景大图上移动界面元素，但是又不想选中底部大图，除了用锁定图层的方法解决这个问题，按Option也能很方便的解决）

![6](/img/article-img/20180820/6.gif)

多图层堆叠的情况

![7](/img/article-img/20180820/7.gif)

多选且不想移动某些元素

3）同时按住option+command可以做到单独移动图层，鼠标焦点可以不在被选图层上，如果不按这2个快捷键组合，在元素区域外是没法移动的，当在界面中有大量图层时，也可以避免误操作到其他图层（笔者强烈推荐，这个组合键经常用到，对于解决选择移动问题非常有帮助）

![8](/img/article-img/20180820/8.gif)

4）如果有重叠图层，尤其是上层把下层遮住时，要直接选择它会比较麻烦，此时可以选择最上层图层右键选择想要的图层，结合前面提到的快捷键进行移动或者修改操作。

![9](/img/article-img/20180820/9.gif)

5）对齐图层

Control-Command-V 垂直方向上的等分；Control-Command-H水平方向上的等分，这个快捷键非常常用，比每次点击右上角的对齐工具要方便很多。

6）调整图层

对图层放大缩小是一个经常需要用到的操作，但是如果某些图层带有图层样式，比如描边，投影，圆角这些，在直接缩放时并不能同时缩放，比如把长宽各位50px且描边为10px的形状改为长宽100px的形状时，其描边还是为10px。那怎么解决这个问题呢？

其实sketch是有2种缩放形式，一种是直接缩放，不改变元素样式只修改基本属性大小；另一种是变换缩放，可以同时缩放基本属性以及样式属性。操作方式是从菜单中选择“ **图层”>“变换”>“缩放...** ”（或按Command-K），这个对symbol也有效果。

![10](/img/article-img/20180820/10.gif)

#### 3、图层约束技巧

首先看看什么是图层约束，直接看图吧，图层约束能做到下面这种效果：

![11](/img/article-img/20180820/11.gif)

在做界面适配的时候是不是很方便，那具体如何做到呢？

1）图层缩放固定边距

在元素属性栏，可以找到约束设置，根据需要设置子元素与父元素之间的关系（注意事项，图层约束必须是建立在图层组中，如果没有组的概念，则无法使用图层约束；子父级关系是指参照关系，比如下图中白色块相对于底部的蓝色块，白色就是子级，蓝色就是父级，而对resizing的设置其实就是设置子级）

![12](/img/article-img/20180820/12.gif)

子父级关系

![13](/img/article-img/20180820/13.gif)

Apple官方组件关于图层约束的设置

2）symbol内容自动适应

在输入项里有光标的情况下，能自动根据内容长短改变位置

![14](/img/article-img/20180820/14.gif)

#### 4、图形操作技巧

旋转是需要经常用到的操作，在sketch中也是有很多方式可以实现图层旋转，需要看情况来使用。

1）通过属性栏的角度设置直接设置圆角值，在旋转角度很明确的时候很方便

![15](/img/article-img/20180820/15.png)

2）通过工具栏上的旋转选项进行旋转，优点是选择后可以在画面上任何位置对对象进行旋转

![16](/img/article-img/20180820/16.png)

3）直接通过快捷键实现旋转，按住command健并拖动对象其中一个控制柄即可旋转，这个快捷操作，在需要多频次调整旋转时，会很实用。

![17](/img/article-img/20180820/17.gif)

4）另外，补充一点旋转以外的小知识，在做变换的时候，comand健也很有用。它可以让对象变换只从一个方向上调整。

![18](/img/article-img/20180820/18.gif)

#### 5、蒙版技巧

1）在sketch中的蒙版功能很强大，不光对图层可以使用蒙版，对图层组也可以使用，但在蒙版组内，新建任何图层或者图层组都会被自动蒙版，有时候反而会成为麻烦。

有2种办法可以解除蒙版。1是把图层或组拖出蒙版组之外，但是这样会破坏元素结构；2是直接选择想要解除的图层，右键忽略底层蒙版即可，这样做的好处是，可以不会破坏对象组织结构。

![19](/img/article-img/20180820/19.gif)

2）在sketch中有2种形式的蒙版，一种是基于图形，另一种是基于透明度来实现的，常用渐变来做图片渐隐效果。这2个都很常用，就不过多赘述。

#### 6、sketch文件压缩

在源文件中适用很多高清图后，往往会让整个sketch文件变的很大，一是传输不方便，另一个也会导致文件卡顿，反应慢。此时可以使用图层-图片-最小尺寸来对文件进行快速压缩。

![20](/img/article-img/20180820/20.png)

#### 7、批量替换颜色

在进行多页面多画板修改颜色时，在不是symbol的情况下，修改起来会很费时间。其实sketch内置了批量修改颜色功能，只是可能用的人不多。

具体操作为：编辑——查找并替换颜色（option+command+F），需要注意颜色透明度，根据实际需要判断是否勾选。

![21](/img/article-img/20180820/21.gif)

图片来源：sketch官网

#### 8、快捷切换视图

设计过程中，需要经常切换不同视图来查看设计内容，简直超高频的使用需求！所以对于这些快捷键必须要在这里提一句：

Command +1 完整展示页面里的所有内容，适合全局展示，查看一致性。

![22](/img/article-img/20180820/22.jpg)

Command +2 将选中的元素放大到合适屏幕的尺寸，这个视图有一个妙用就是可以把复制的元素直接复制到当前元素的中间，这个特性非常实用，自己试过就知道了，肯定会有用到的地方。

![23](/img/article-img/20180820/23.jpg)

Command +3 将选中的元素显示在屏幕中央

![24](/img/article-img/20180820/24.jpg)

Command + 0 以实际像素模式预览页面，即在100%大小下看设计效果

![25](/img/article-img/20180820/25.jpg)

#### 9、图层对齐

图层对齐也是经常要用到的操作。直接与对象对齐的话，Sketch会将图层对齐到所有选定对象的最外层。但要将图层与特定对象对齐，怎么操作呢？

比如想让下图中两个元素以正方形为参照物进行居中，那应该先使用图层列表中的锁定按钮或使用Shift-Command-L 锁定该图层，然后再执行对齐操作即可。

![26](/img/article-img/20180820/26.gif)

#### 10、如何sketch形状默认值

刚开始使用sketch时，新建矩形，每次都会自带描边，然后再手动关闭描边，很麻烦。这个默认值能改吗？当然可以。

操作：首先建一个不带描边的矩形，然后选择layer-style-set style as default  （这个功能以前是放在Edit里的，更新后合并到了style中）。搞定，下次再新建形状时就会以你刚设置的样式作为默认值了。

![27](/img/article-img/20180820/27.jpg)



好了，本期sketch冷知识就先介绍到这里，下一期可能会分享symbols和Libraries的相关冷知识，敬请期待~

另外再多说一句，文章中所提到的小技巧，一定要自己动手去试试啊，要不然看过了你也还是用不到，不信？那就试试看。



> 参考文章：https://www.sketchapp.com/docs



