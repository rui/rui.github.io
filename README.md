
本博客基于 [LOFFER](https://fromendworld.github.io/LOFFER/document/)，
这是一个可以发布在GitHub的Jekyll博客，你不需要编写代码或使用命令行即可获得一个部署在GitHub的博客。

* 支持LaTeX渲染数学公式，请见[这篇说明和示例](https://fromendworld.github.io/LOFFER/math-test/)。
* 要更换主题颜色，只要打开文件` _sass/_variables.scss `，将文件中所有的teal全部替换成你想要的颜色。例如，查找teal，替换indigo，全部替换，commit，完成！
* 支持Disqus和Gitalk两种评论区。请在_config.yml中设置。
* 链接博客主的社交媒体。请在_config.yml中填写。
* 按照标签和日期查看博文归档。请查看/tags 和/archive 页面。
* 在 post 的 yaml 头部中加入 `toc: true`， 这篇博文就会显示目录了。
* 在 post 的 yaml 头部中加入 `pinned: true` 就可以置顶博文。


## 博文YAML举例：

    ---
    layout: post
    title: Markdown语法简介
    date: 2013-07-16
    Author: Shengbin 
    tags: [sample, markdown]
    comments: true
    toc: true
    pinned: false
    ---


## 致谢

* [Jekyll](https://github.com/jekyll/jekyll) - 这是本站存在的根基
* [Kiko-now](<https://github.com/aweekj/kiko-now>) - 我首先是fork这个主题，然后再其上进行修改汉化，才有了LOFFER
* [Font Awesome](<https://fontawesome.com/>) - 社交网络图标来自FontAwesome的免费开源内容



## 帮助这个项目

点一个☆吧！

![img](https://raw.githubusercontent.com/FromEndWorld/LOFFER/master/images/givemefive.png)
