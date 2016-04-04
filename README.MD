#FEMore，前端知识汇总

##1、在js中，什么语句可以直接断点？
debugger

##2、i和em有什么区别？
i(italic)单纯表示倾斜，而em(emphasize)是具有语义化的，表示强调的意思，只是浏览器渲染效果也是斜体。
这点从他们各自的单词也可以看得出来。

##3、b和strong有什么区别？
跟上一题一样，前者表示粗体显示。后者具有语义，表示强调，渲染效果跟加粗一样。

##4、<img>的title和alt有什么区别？
title：是属于全局属性。当鼠标移动到某元素上面时，通常会显示该内容。
alt：本属性是img特有的，用于当图片不可用的时候，显示出来的代替文本。

##5、对web语义化有什么看法？
web语义化是指页面代码所蕴含的信息，HTML标签和CSS命名都可以进行语义化。
*有利于搜索引擎理解页面
*便于盲人阅读
如果语义化标签数量大量增长的话（假设），势必会对相关内容进行细化，由此可能造成开发人员在编写代码时会混淆相关标签。

##display: none与visibility: hidden的区别
相同：都让元素不可见
不同：
*display:none，在dom tree与cssom tree合成的layout tree的时候，元素不会被合成到该树上的，所以在布局的时候，不会占空间。
*visibility:hidden：会在layout tree中，所以会占空间，只是内容不可见。
*更改display属性通常会造成内容reflow，而visibility则只会repaint
*display:none的子节点也会从layout tree树中消失，而visibility还可以设置子节点可见。
