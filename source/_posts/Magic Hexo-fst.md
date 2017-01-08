---
title: 'Magic Hexo-fst'
tags: Hexo
---
# Magic Hexo-fst
## ——简单分享Hexo的配置与部署


### 一丢丢吐槽与建议
首先声明一点，本文不仅是教你如何去安装配置以及部署Hexo，更多的是分享一下小白搭建时的一丢丢经验。小白也不建议大家通过网上的各种奇葩教程学习如何搭建自己的Hexo博客，希望大家可以学习阅读[Hexo说明文档](https://hexo.io/zh-cn/docs/index.html "Hexo")（感觉更有用）来解决你可能遇到的问题。
<!-- more -->

## 言归正传
### Hexo是什么
简而言之，Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他渲染引擎）解析文章，在几秒 内，即可利用靓丽的主题生成静态网页。

### 搭建
再次强调[Hexo说明文档](https://hexo.io/zh-cn/docs/index.html "Hexo")的重要性，如果接下来的步骤不适用你，赶紧去看说明文档吧 -、 -

#### 安装 Hexo
安装 Hexo 相当简单。然而在安装前，您必须检查电脑中是否已安装下列应用程序：
[Node.js](https://nodejs.org/)
[Git](http://git-scm.com/)
如果您的电脑中已经安装上述必备程序，那么恭喜您！接下来只需要使用 npm 即可完成 Hexo 的安装。
`$ npm install -g hexo-cli`
如果没有安装，自行参见[Hexo说明文档](https://hexo.io/zh-cn/docs/index.html "Hexo")。

#### 建站
安装 Hexo 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。
	$ hexo init
	$ cd
	$ npm install
新建完成后，指定文件夹的目录如下：
	├── _config.yml
	├── package.json
	├── scaffolds
	├── scripts
	├── source |
	├── _drafts |
	└── _posts
	└── themes
至于每一个文件夹是干嘛滴，So easy，看说明文档啊。
这里只说说 _config.yml _ ，就是他，我们站点的配置文件，里面有许多好玩的参数，你可以参见说明文档改改，相信你会有更深刻的理解。
对咯，其中给大家推荐一款 _theme：_  [scheme of next](http://theme-next.iissnan.com/) ，非常简约漂亮，反正我是非常喜欢哈，我的[博客](blog.legendqmz.cn)用的就是这款scheme。

在本地修改完这一连串的配置，（包括：语言设置、财产、菜单设置、侧栏设置、头像设置、作者名称、站点描述、标签云页面、分类页面、统计系统、评论系统等等）现在是需要下面的一个命令即可在本地成功预览你的博客样式。完成之后你就可以开启本地测试浏览你的成果咯，其命令如下
	$ hexo c
	$ hexo g
	$ hexo s #启动本地服务器测试
这个时候在浏览器中输入http://localhost:4000 静态的网站架设完成！

#### Conclusion
非常简单吧，这样你本地博客的搭建就宣告完成啦。
下次再分享如何讲本地博客部署到你的服务器上咯。_See you again_
