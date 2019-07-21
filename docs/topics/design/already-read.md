
# 设计一个新闻列表，用户已经看过的新闻，在标题后面增加“已阅读”文字

## 问题描述

现在有这样一个新闻列表，用户点击新闻可以看详情。
但是回来的时候，用户并不知道刚才看了什么，影响效率。
因此想做一个“在已经看过的新闻标题后面增加“已阅读”文字”的功能。

## 关键点

这是一个相当开放的问题。 这个描述信息不够，我们需要通过“追问”的
方式来获取更多信息。 我们需要综合多种方案，作出一个综合的整理，各个方案的
优缺点是什么，最后结合实际情况敲定一个方案。

技术上，我们有多种方法实现：

1. 后端加一个字端，前端根据数据不同展示不同的样式

2. 前端持久化存储，前端根据数据不同展示不同的样式

3. 前端通过CSSvisited伪类，给已经点击的标题增加特殊样式（但是似乎无法增加文字）

然后我们其实需要更多信息帮我们决策，因此需要追问一些其他信息辅助我们决策，比如：

- 这个项目的用户量有多大？PV多少？

- 需要做到精确么，比如用户换了手机，清了缓存要确保功能不受影响么？

- 是否可以换成别的交互形式，比如看过的标题改为特别的样式？（对应我们的方案3）


当你听到这三个答案的话，就可以做方案了。