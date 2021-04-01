---
title: 块级&行内元素
---
# HTML

HTML4中，元素被分成两大类: inline(内联元素)与block(块级元素)。但在实际的开发过程中，因为页面表现的需要，前端工程师经常把inline元素的display值设定为block(比如a标签)，也经常把block元素的display值设定为inline；之后更是出现了inline-block这一对外呈现inline、对内呈现block的属性。因此，简单地把HTML元素划分为inline与block已经不再符合实际需求。

基于这种考虑，在HTML5中，标准制定者重新定义了HTML元素的分类，并根据这一新的分类定义了元素的内容模型(Content Model) -- 对于一个元素而言，哪些子元素是合法的，而哪些子元素是非法的。

但是还是列一下出来，这个概念比HTML5中的分类容易理解得多。
<!-- more -->
## 块级元素

- 格式

  默认情况下，块级元素会新起一行。

- 内容模型

  一般块级元素可以包含行内元素和其他块级元素。这种结构上的包含继承区别可以使块级元素创建比行内元素更”大型“的结构。

HTML 标准中块级元素和行内元素的区别至高出现在 4.01 标准中。在 HTML5，这种区别被一个更复杂的[内容类别](https://developer.mozilla.org/zh-CN/docs/HTML/Content_categories)代替。”块级“类别大致相当于 HTML5 中的[流内容](https://developer.mozilla.org/zh-CN/docs/HTML/Content_categories#Flow_content)类别，而”行内“类别相当于 HTML5 中的[措辞内容](https://developer.mozilla.org/zh-CN/docs/HTML/Content_categories#Phrasing_content)类别，不过除了这两个还有其他类别。

| 标签                                                         | 说明                                                         | 备注  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ----- |
| [`<address>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/address) | 联系方式信息                                                 |       |
| [`<article>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/article) | 文章内容                                                     | HTML5 |
| [`<aside>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/aside) | 伴随内容                                                     | HTML5 |
| [`<audio>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/audio) | 音频播放                                                     | HTML5 |
| [`<blockquote>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/blockquote) | 块引用                                                       |       |
| [`<canvas>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/canvas) | 绘制图形                                                     | HTML5 |
| [`<dd>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dd) | 定义列表中定义条目描述                                       |       |
| [`<div>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/div) | 文档分区                                                     |       |
| [`<sl>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dl) | 定义列表                                                     |       |
| [`<fieldset>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/fieldset) | 表单元素分组                                                 |       |
| [`<figcaption>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/figcaption) | 图文信息组标题                                               | HTML5 |
| [`<figure>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/figure) | [图文信息组   (参照 )](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/figcaption) | HTML5 |
| [`<footer>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/footer) | 区段尾或页尾                                                 | HTML5 |
| [`<form>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/form) | 表单                                                         |       |
| [`<h1>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h1), [`<h2>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h2), [`<h3>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h3), [`<h4>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h4), [`<h5>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h5), [`<h6>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/h6) | 标题级别 1-6.                                                |       |
| [`<header>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/header) | 区段头或页头                                                 | HTML5 |
| [`<hgroup>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/hgroup) | 标题组                                                       | HTML5 |
| [`<hr>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/hr) | 水平分割线                                                   |       |
| [`<noscript>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/noscript) | 不支持脚本或禁用脚本时显示的内容                             |       |
| [`<ol>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/ol) | 有序列表                                                     |       |
| [`<output>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/output) | 表单输出                                                     | HTML5 |
| [`<p>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/p) | 行                                                           |       |
| [`<pre>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/pre) | 预格式化文本                                                 |       |
| [`<section>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/section) | 一个页面区段                                                 | HTML5 |
| [`<table>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/table) | 表格                                                         |       |
| [`<tfoot>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/tfoot) | 表脚注                                                       |       |
| [`<ul>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/ul) | 无序列表                                                     |       |
| [`<video>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/video) | 视频                                                         | HTML5 |

## 行内元素

https://developer.mozilla.org/zh-CN/docs/Web/HTML/Inline_elements

 - 内容

一般情况下，行内元素只能包含数据和其他行内元素。

而块级元素可以包含行内元素和其他块级元素。这种结构上的包含继承区别可以使块级元素创建比行内元素更”大型“的结构。

 - 格式

默认情况下，行内元素不会以新行开始，而块级元素会新起一行。

- [b](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/b), [big](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/big), [i](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/i), [small](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/small), [tt](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/tt)
- [abbr](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/abbr), [acronym](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/acronym), [cite](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/cite), [code](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/code), [dfn](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dfn), [em](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/em), [kbd](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/kbd), [strong](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/strong), [samp](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/samp), [var](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/var)
- [a](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/a), [bdo](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/bdo), [br](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/br), [img](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/img), [map](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/map), [object](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/object), [q](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/q), [script](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script), [span](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/span), [sub](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/sub), [sup](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/sup)
- [button](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/button), [input](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input), [label](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/label), [select](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/select), [textarea](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/textarea)

## HTML5 中的分类方式

## 置换元素

深入前端之replaced element https://juejin.cn/post/6844903775354748936 

在 [CSS](https://developer.mozilla.org/zh-CN/docs/Web/CSS) 中，**可替换元素**（**replaced element**）的展现效果不是由 CSS 来控制的。这些元素是一种外部对象，它们外观的渲染，是独立于 CSS 的。

简单来说，它们的内容不受当前文档的样式的影响。CSS 可以影响可替换元素的位置，但不会影响到可替换元素自身的内容。某些可替换元素，例如 [`<iframe>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe) 元素，可能具有自己的样式表，但它们不会继承父文档的样式。

CSS 能对可替换元素产生的唯一影响在于，部分属性支持控制元素内容在其框中的位置或定位方式。有关详细信息，请参阅本文下面的[控制内容框中的对象位置](https://developer.mozilla.org/zh-CN/docs/Web/CSS/Replaced_element#控制内容框中的对象位置)。

https://developer.mozilla.org/zh-CN/docs/Web/CSS/Replaced_element

典型的可替换元素有：

- [`<iframe>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe)
- [`<video>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/video)
- [`<embed>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/embed)
- [`<img>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/img)

有些元素仅在特定情况下被作为可替换元素处理，例如：

- [`<option>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/option)
- [`<audio>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/audio)
- [`<canvas>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/canvas)
- [`<object>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/object)
- [`<applet>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/applet)

HTML 规范也说了 [`<input>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input) 元素可替换，因为 `"image"` 类型的 [`<input>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input) 元素就像[`img`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/img)一样被替换。但是其他形式的控制元素，包括其他类型的 [`input`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/Input) 元素，被明确地列为非可替换元素（non-replaced elements）。该规范用术语小挂件（Widgets）来描述它们默认的限定平台的渲染行为。

用 CSS [`content`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/content) 属性插入的对象是匿名的可替换元素。它们并不存在于 HTML 标记中，因此是“匿名的”。

# CSS

## 块级框

## 行内框
不允许设置宽和高
## 行内块级框



## 参考

参考：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Block-level_elements

http://blog.shaochuancs.com/w3c-html5-content-model/

https://www.zhihu.com/question/34952563

http://happylg.cn/2017/09/22/block-and-inline/

https://www.cnblogs.com/zhuzhenwei918/p/6389567.html

http://blog.doyoe.com/2015/03/15/css/%E7%BD%AE%E6%8D%A2%E5%92%8C%E9%9D%9E%E7%BD%AE%E6%8D%A2%E5%85%83%E7%B4%A0/

http://blog.doyoe.com/2015/03/09/css/%E8%A7%86%E8%A7%89%E6%A0%BC%E5%BC%8F%E5%8C%96%E6%A8%A1%E5%9E%8B%E4%B8%AD%E7%9A%84%E5%90%84%E7%A7%8D%E6%A1%86/#block-level-element
