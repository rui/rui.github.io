---
layout: page
title: 关于
permalink: /
---

毕业于[中国科学技术大学](http://www.ustc.edu.cn){:target="_blank"}，
专业是[计算数学](http://math.ustc.edu.cn){:target="_blank"}，
爱好**计算机编程**。
在这里分享一些我的学习心得。

本人的研究方向是**高精度数值格式**。

<div class="publications">
<h6> 论文 </h6>
<ol>
{% for ref in site.data.cv-publications %}
  <li> <span class="author">{{ ref.authors | join: " , " }}</span>, <b class="title"> {{ref.title}} </b>, <i class="journal"> {{ ref.journal }}</i>, <b>{{ref.volume}}</b>({{ref.year}}), PP.{{ref.pages}} </li>
{% endfor %}
</ol>
</div>
