---
layout: post
title: "ImagicK剪裁图片"
date: 2022-07-16
categories: [图像处理]
tags: [imagick]
toc: false
pin: false
---

用 ImagicK 的命令行来剪裁图片
```
convert original.png -crop 640x480+50+100 out.png
```
其中，640x480是剪裁的大小，(50,100)是开始的位置。 out.png 是输出文件

另外，还可以增加透明色。

把white+10%色差范围的都设置为透明transparent，
```
convert image.gif -fuzz 10% -transparent white result.gif
```
注意， jpg 文件是不能透明显示的，png文件可以。