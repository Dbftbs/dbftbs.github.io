---
layout: post
title: "Hello World!"
description: "This is the Test file for Jekyll Blog."
category: Demo
tags: [Blog, Markdown, Jekyll]
---
{% include blog/setup %}



Hello, I am Dbftbs.  :-)

This is my personal Blog.

When you see this post, that means my blog is built successfully!

I write this page to test blog features.

First, Let's C(say) `Hello World`.

{% highlight c linenos %}

#include <stdio.h>

int main(void)
{
	printf("Hello World!\n");
	return 0;
}

{% endhighlight %}

<!-- more -->

- - -

*Block Elements*
================

*Headers*
---------

_**Setext Style**_

This is H1
==========

This is H2
----------

_**atx Style**_

# Header 1

## Header 2

### Header 3

#### Header 4 ####

##### Header 5 #####

###### Header 6 ######

* * *

*Blockquotes*
-------------

> Stray birds of summer come to my window to sing and fly away.   
> And yellow leaves of autumn, which have no songs, flutter and fall there with a sign. 

> Shall I compare thee to a summer's day?  
Thou art more lovely and more temperate:  
Rough winds do shake the darling buds of May,  
And summer's lease hath all too short a date:  
Sometime too hot the eye of heaven shines,  
And often is his gold complexion dimm'd;  
And every fair from fair sometime declines,  
By chance or nature's changing course untrimm'd  
But thy eternal summer shall not fade  
Nor lose possession of that fair thou owest;  
Nor shall Death brag thou wander'st in his shade,  
When in eternal lines to time thou growest:  
So long as men can breathe or eyes can see,  
So long lives this and this gives life to thee.  


> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");


*Lists*
-------

### *Unordered lists* ###

* Red
* Green
* Blue

+ X
+ Y
+ Z

- Σωκράτης
- Πλάτων
- Αριστοτέλης

### *Ordered lists* ###

1. C
2. C++
3. Python

- - -

*Tables*
--------

洛书:

4 ||| 9 ||| 2
3 ||| 5 ||| 7
8 ||| 1 ||| 6

<br />
Aligin example (Excerpt from __*Compilers.Principles.Techniques.And.Tools*__):

| LEXEMES      | TOKEN NAME |     ATTRIBUTE VALUE    |
| :----------- | :--------: | ---------------------: |
| Any *ws*     |     --     |                   --   |
| if           |     if     |                   --   |
| then         |    then    |                   --   |
| else         |    else    |                   --   |
| Any *id*     |     id     | Pointer to table entry |
| Any *number* |   number   | Pointer to table entry |
| <            |    relop   |                   LT   |
| <=           |    relop   |                   LE   |
| =            |    relop   |                   EQ   |
| <>           |    relop   |                   NE   |
| >            |    relop   |                   GT   |
| >=           |    relop   |                   GE   |

- - -

*Code Blocks*
-------------

Here is the [Rust](http://www.rust-lang.org/) Programming example(from Rust Home Page).

	// This code is editable and runnable!
	fn main() {
	    // A simple integer calculator:
	    // `+` or `-` means add or subtract by 1
	    // `*` or `/` means multiply or divide by 2

	    let program = "+ + * - /";
	    let mut accumulator = 0;

	    for token in program.chars() {
	        match token {
	            '+' => accumulator += 1,
	            '-' => accumulator -= 1,
	            '*' => accumulator *= 2,
	            '/' => accumulator /= 2,
	            _ => { /* ignore everything else */ }
	        }
	    }

	    println!("The program \"{}\" calculates the value {}",
	              program, accumulator);
	}



- - -

*Horizontal Rules*
------------------

* * *

***

*****

- - -

---------------------------------------



- - -

*Span Elements*
===============

*Links*
-------

Here is my [Blog](http://dbftbs.xyz/ "Dbftbs's Blog")

Here is my [GitHub](https://github.com/Dbftbs)

GitHub Page: <http://dbftbs.github.io>

This is another link of my blog [Link][blog].

See my [About]({{ site.url }}/about.html) page for details.

This is Footnote Test.[^footnote]

Goto [Tag](#TAG)

Goto [Headers](#headers)

*Image*
-------

![View]({{ ASSET_PATH }}/image/jpg/Mountain_landscape.jpg)

![Blogging](http://imgs.xkcd.com/comics/blogging.png "Blogging - image from xkcd")


*Emphasis*
----------

*single asterisks*

_single underscores_

**double asterisks**

__double underscores__



*Code*
------

Use the `int printf(const char *format, ...);` function.

``There is a literal backtick (`) here.``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

This is a  `<br />` tags.

- - -

*Backlash Escapes*
------------------

Markdown allows you to use backslash escapes to generate literal characters which would otherwise have special meaning in Markdown’s formatting syntax. For example, if you wanted to surround a word with literal asterisks (instead of an HTML <em> tag), you can use backslashes before the asterisks, like this:

2015\. 07

\*literal asterisks\*

Markdown provides backslash escapes for the following characters:

\   backslash
`   backtick
*   asterisk
_   underscore
{}  curly braces
[]  square brackets
()  parentheses
#   hash mark
+   plus sign
-   minus sign (hyphen)
.   dot
!   exclamation mark


*Other*
=======

*Inline HTML*
-------------

This is a <a id="TAG">Tag</a>.

*MathJax*
---------

{% include blog/latex_support %}

You can render *LaTeX* mathematical expressions using **MathJax**, as on [math.stackexchange.com][1]:

The *Gamma function* satisfying $$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$$ is via the Euler integral

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

- - -

*中文测试*
---------

**千字文**

*梁 周兴嗣*

	天地玄黄 宇宙洪荒
	日月盈昃 辰宿列张
	寒来暑往 秋收冬藏
	闰余成岁 律吕调阳
	云腾致雨 露结为霜
	金生丽水 玉出昆冈
	剑号巨阙 珠称夜光
	果珍李柰 菜重芥姜
	海咸河淡 鳞潜羽翔
	龙师火帝 鸟官人皇
	始制文字 乃服衣裳
	推位让国 有虞陶唐
	吊民伐罪 周发殷汤
	坐朝问道 垂拱平章
	爱育黎首 臣伏戎羌
	遐迩一体 率宾归王
	鸣凤在竹 白驹食场
	化被草木 赖及万方
	盖此身发 四大五常
	恭惟鞠养 岂敢毁伤
	女慕贞洁 男效才良
	知过必改 得能莫忘
	罔谈彼短 靡恃己长
	信使可覆 器欲难量
	墨悲丝染 诗赞羔羊
	景行维贤 克念作圣
	德建名立 形端表正
	空谷传声 虚堂习听
	祸因恶积 福缘善庆
	尺璧非宝 寸阴是竞
	资父事君 曰严与敬
	孝当竭力 忠则尽命
	临深履薄 夙兴温凊
	似兰斯馨 如松之盛
	川流不息 渊澄取映
	容止若思 言辞安定
	笃初诚美 慎终宜令
	荣业所基 籍甚无竟
	学优登仕 摄职从政
	存以甘棠 去而益咏
	乐殊贵贱 礼别尊卑
	上和下睦 夫唱妇随
	外受傅训 入奉母仪
	诸姑伯叔 犹子比儿
	孔怀兄弟 同气连枝
	交友投分 切磨箴规
	仁慈隐恻 造次弗离
	节义廉退 颠沛匪亏
	性静情逸 心动神疲
	守真志满 逐物意移
	坚持雅操 好爵自縻
	都邑华夏 东西二京
	背邙面洛 浮渭据泾
	宫殿盘郁 楼观飞惊
	图写禽兽 画彩仙灵
	丙舍旁启 甲帐对楹
	肆筵设席 鼓瑟吹笙
	升阶纳陛 弁转疑星
	右通广内 左达承明
	既集坟典 亦聚群英
	杜稿钟隶 漆书壁经
	府罗将相 路侠槐卿
	户封八县 家给千兵
	高冠陪辇 驱毂振缨
	世禄侈富 车驾肥轻
	策功茂实 勒碑刻铭
	磻溪伊尹 佐时阿衡
	奄宅曲阜 微旦孰营
	桓公匡合 济弱扶倾
	绮回汉惠 说感武丁
	俊义密勿 多士实宁
	晋楚更霸 赵魏困横
	假途灭虢 践土会盟
	何遵约法 韩弊烦刑
	起翦颇牧 用军最精
	宣威沙漠 驰誉丹青
	九州禹迹 百郡秦并
	岳宗泰岱 禅主云亭
	雁门紫塞 鸡田赤城
	昆池碣石 钜野洞庭
	旷远绵邈 岩岫杳冥
	治本于农 务兹稼穑
	俶载南亩 我艺黍稷
	税熟贡新 劝赏黜陟
	孟轲敦素 史鱼秉直
	庶几中庸 劳谦谨敕
	聆音察理 鉴貌辨色
	贻厥嘉猷 勉其祗植
	省躬讥诫 宠增抗极
	殆辱近耻 林皋幸即
	两疏见机 解组谁逼
	索居闲处 沉默寂寥
	求古寻论 散虑逍遥
	欣奏累遣 戚谢欢招
	渠荷的历 园莽抽条
	枇杷晚翠 梧桐蚤凋
	陈根委翳 落叶飘摇
	游鹍独运 凌摩绛霄
	耽读玩市 寓目囊箱
	易輶攸畏 属耳垣墙
	具膳餐饭 适口充肠
	饱饫烹宰 饥厌糟糠
	亲戚故旧 老少异粮
	妾御绩纺 侍巾帷房
	纨扇圆洁 银烛炜煌
	昼眠夕寐 蓝笋象床
	弦歌酒宴 接杯举觞
	矫手顿足 悦豫且康
	嫡后嗣续 祭祀烝尝
	稽颡再拜 悚惧恐惶
	笺牒简要 顾答审详
	骸垢想浴 执热愿凉
	驴骡犊特 骇跃超骧
	诛斩贼盗 捕获叛亡
	布射僚丸 嵇琴阮啸
	恬笔伦纸 钧巧任钓
	释纷利俗 并皆佳妙
	毛施淑姿 工颦妍笑
	年矢每催 曦晖朗曜
	璇玑悬斡 晦魄环照
	指薪修祜 永绥吉劭
	矩步引领 俯仰廊庙
	束带矜庄 徘徊瞻眺
	孤陋寡闻 愚蒙等诮
	谓语助者 焉哉乎也




- - -

[^footnote]: Here is the *text* of the **footnote**.

[blog]: <http://blog.dbftbs.xyz/>  "Dbftbs's Blog"



