---
layout: post
title: "ImagicK放缩图片"
date: 2022-10-03
categories: [图像处理]
tags: [imagick]
toc: false
pin: false
---

在 Imagick 中，使用`-resize`来放缩图片到指定的大小。

<!-- more -->

用 ImagicK 的命令行来放缩图片到指定大小
```
convert logo.png -resize 64x64 favicon.ico
```
会把图像保持原来的放缩比放到`64x64`大小的图形内。
本例中，也就是宽或者高最多是64。

如果想拉伸原图，强行放缩到指定大小，可以加上`!`
```
convert logo.png -resize 64x64\! favicon.ico
```
这时，图片可能会变形。

还有如 `^`, `>`, `<` 等操作，可以参考[ImageMagick](https://legacy.imagemagick.org/Usage/resize/)


