# 数据结构

> 教程原件：《大话数据结构》
>
> [If you give someone a program, you will frustrate them for a day;](如果你交给某人一个程序，你将折磨他一整天)
> [if you teach them how to program, you will frustrate them for a lifetime.](如果你教会他编写程序，那么你将会折磨他一辈子。)

## 数据结构起源

早期人们都把计算机理解为数值计算工具,就是感觉计算机当然是用来计算的, 所以计算机解决问题,应该是先从具体问题中抽象出一个适当的数据模型,设计出 个解此数据模型的算法,然后再编写程序,得到一个实际的软件。

可现实中,我们更多的不是解决数值计算的问题,而是需要一些更科学有效的手 段(比如表、树和图等数据结构)的帮助,才能更好地处理问题。**所以数据结构是一 门研究非数值计算的程序设计问题中的操作对象,以及它们之间的关系和操作等相关 问题的学科。**

## 基本概念和术语

> 说到数据结构是什么,我们得先来谈谈什么叫数据。
>
> 正所谓“巧妇难为无米之炊”,再强大的计算机,也是要有“米”下锅才可以干活 的,否则就是一堆破铜烂铁。这个“米”就是数据。

### 数据

数据:**是描述客观事物的符号,是计算机中可以操作的对象,是能被计算机识 别,并输入给计算机处理的符号集合。数据不仅仅包括整型、实型等数值类型,还包 括字符及声音、图像、视频等非数值类型。**

比如我们现在常用的搜素引擎,一般会有网页、MP3、图片、视频等分类。MP3

就是声音数据,图片当然是图像数据,视频就不用说了,而网页其实指的就是全部数 据的搜索,包括最重要的数字和字符等文字数据。

也就是说,我们这里说的数据,其实就是符号,而且这些符号必须具备两个前提：

```markdown
- 可以输入到计算机中。 
- 能被计算机程序处理。
```

对于整型、实型等数值类型,可以进行数值计算。

对于字符数据类型,就需要进行非数值的处理。而声音、图像、视频等其实是可 以通过编码的手段变成字符数据来处理的。

### 数据元素

数据元素:是组成数据的、有一定意义的基本单位,在计算机中通常作为整体处理。也被称为记录。

比如,在人类中,什么是数据元素呀?当然是人了。

畜类呢?哈,牛、马、羊、鸡、猪、狗等动物当然就是禽类的数据元素。

### 数据项

数据项:**一个数据元素可以由若干个数据项组成。**

比如人这样的数据元素,可以有眼、耳、鼻、嘴、手、脚这些数据项,也可以有 姓名、年龄、性别、出生地址、联系电话等数据项,具体有哪些数据项,要视你做的 系统来决定。

数据项是数据不可分割的最小单位。在数据结构这门课程中,我们把数据项定义 为最小单位,是有助于我们更好地解决问题。所以,记住了,数据项是数据的最小单 位。但真正讨论问题时,数据元素才是数据结构中建立数据模型的着眼点。就像我们 讨论一部电影时,是讨论这部电影角色这样的“数据元素”,而不是针对这个角色的姓 名或者年龄这样的“数据项”去研究分析。

### 数据对象

数据对象:是性质相同的数据元素的集合,是数据的子集

什么叫性质相同呢,是指数据元素具有相同数量和类型的数据项,比如,还是刚 才的例子,人都有姓名、生日、性别等相同的数据项

既然数据对象是数据的子集,在实际应用中,处理的数据元素通常具有相同性 质,在不产生混淆的情况下,我们都将数据对象简称为数据。

### 数据结构

结构,简单的理解就是关系,比如分子结构,就是说组成分子的原子之间的排列 方式。严格点说,结构是指各个组成部分相互搭配和排列的方式。在现实世界中,不 同数据元素之间不是独立的,而是存在特定的关系,我们将这些关系称为结构。那数 据结构是什么?

数据结构:**是相互之间存在一种或多种特定关系的数据元素的集合。 **

在计算机中,数据元素并不是孤立、杂乱无序的,而是具有内在联系的数据集合。数据元素之间存在的一种或多种特定关系,也就是数据的组织形式。

为编写出一个“好”的程序,必须分析待处理对象的特性及各处理对象之间存在的关系。这也就是研究数据结构的意义所在。