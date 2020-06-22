
[TOC]

## 1.特殊字符自动转义
&lt; 和 &amp;  必须将它们转义为字符实体

Markdown中的转义字符为\，转义的有：
\ 反斜杠 ` 反引号 * 星号 _ 下划线 {} 大括号 [] 中括号 () 小括号  # 井号 + 加号 - 减号 . 英文句号 ! 感叹号

## 2.多种注释格式，不会显示
<div style='display: none'>
哈哈我是注释，不会在浏览器中显示。
</div>

<!--哈哈我是注释，不会在浏览器中显示。-->

<!--
哈哈我是多段注释，
不会在浏览器中显示。
-->

[//]: # (哈哈我是最强注释，不会在浏览器中显示。)
[^_^]: # (哈哈我是最萌注释，不会在浏览器中显示。)
[//]: <> (哈哈我是注释，不会在浏览器中显示。)
[comment]: <> (哈哈我是注释，不会在浏览器中显示。)


## 3.标题
<!-->
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题  <!--最多6级标题-->



## 4.任务列表
- [ ] 任务一 未做任务 `- + 空格 + [ ]`
- [x] 任务二 已做任务 `- + 空格 + [x]`

## 5.缩进、换行、空行、对齐方式
【1】 &emsp;或&#8195; //全角
【2】 &ensp;或&#8194; //半角
【3】 &nbsp;或&#160;  //半角之半角

有的编辑器换行必须得在一行字后面空两个格子才行

<center>行中心对齐</center>
<p align="left">行左对齐</p>
<p align="right">行右对齐</p>

## 6.斜体、粗体、删除线、下划线、背景高亮
*斜体*
**粗体**
***加粗斜体***
~~删除线~~
++下划线++
==背景高亮==

## 7.超链接、页内链接、自动链接、注脚
**行内式**  欢迎阅读[择势勤](https://www.jianshu.com/u/16d77399d3a7 "择势勤")

**参考式**  我经常去的几个网站[Google][1]、[Leanote][2]。
[1]:http://www.google.com 
[2]:http://www.leanote.com



&lt;http://example.com/&gt; &emsp;&emsp; 
&lt;address@example.com&gt;


## 8.无序列表、有序列表、定义型列表
* 无序列表项 一
+ 无序列表项 二
+ 无序列表项 二
- 无序列表项 三

1. 有序列表项 一
2. 有序列表项 二
3. 有序列表项 三

:   轻量级文本标记语言（左侧有一个可见的冒号和四个不可见的空格）


## 9.图片
<center>  <!--开始居中对齐-->

![GitHub set up](http://zh.mweb.im/asset/img/set-up-git.gif "图片Title")
格式: ![图片Alt](图片地址 "图片Title")
</center> <!--结束居中对齐-->


## 10.多级引用
>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白


## 11.字体、字号、颜色
<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=#0099ff size=12 face="黑体">黑体</font>
<font color=gray size=5>gray</font>
<font color=#00ffff size=3>null</font>


## 12.代码块
C语言里的函数 `scanf()` 怎么使用？

```
#include stdio.h
int main(void)
{
    printf(&#34;Hello world\n&#34;);
}
```

## 13.表格
|学号|姓名|序号|
|-|-|-|
|小明明|男|5|
|小红|女|79|
|小陆|男|192|


## 14.公式
质能守恒方程可以用一个很简洁的方程式 `$E = m c^2 $`来表达。

```math
E = mc^2
```

```math
x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} 
```
```math
[\frac{1}{\Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{\frac25 \pi}} =
1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {1+\frac{e^{-6\pi}}
{1+\frac{e^{-8\pi}} {1+\ldots} } } }]
```

## 15.分隔线
* * *
***
*****
- - -
----------


## 16. html源码
第一个例子：
<div class="footer">
© 2004 Foo Corporation
</div>
第二个例子：
<center>

<table>
<tr>
<th rowspan="2">值班人员</th>
<th>星期一</th>
<th>星期二</th>
<th>星期三</th>
</tr>
<tr>
<td>李强</td>
<td>张明</td>
<td>王平</td>
</tr>
</table>

</center>

## 17.特殊字
<center>

特殊字符	描述	字符的代码
空格符	&nbsp;
<	小于号	&lt;
>	大于号	&gt;
&	和号	&amp;
￥	人民币	&yen;
©	版权	&copy;
®	注册商标	&reg;
°C	摄氏度	&deg;C
±	正负号	&plusmn;
×	乘号	&times;
÷	除号	&divide;
²	平方（上标²）	&sup2;
³	立方（上标³）	&sup3;
</center>
