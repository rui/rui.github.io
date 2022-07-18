---
layout: post
title: "第二型曲面积分"
date: 2022-07-18
categories: [数学, 高等数学]
tags: [calculus, 第二型曲面积分]
toc: false
pin: false
---


**问：**{: .example-title}
$S$是椭球面$\displaystyle \frac{x^2}{4}+\frac{y^2}{4}+\frac{(z-1)^2}{9}=1$在平面$z=2$和$z=-2$之间的部分，方向是外侧。
计算曲面积分$\displaystyle I=\iint_S \frac{ xdydz+ydzdx+zdxdy}{(x^2+y^2+z^2)^{\frac{3}2}}$。
{:.example}

<!-- more -->

<!-- 上面的是摘要分割线 -->

<div class="solution">
<strong class="soln-title">解：</strong>
注意到
$$
P'_x=\frac1{(x^2+y^2+z^2)^3}\left((x^2+y^2+z^2)^{\frac32}-x\frac32(x^2+y^2+z^2)^{\frac12}2x\right)
=\frac{y^2+z^2-2x^2}{(x^2+y^2+z^2)^3}
$$
因而，
$$
P'_x+Q'_y+R'_z=0
$$
注意到$P$,$Q$, $R$在$(0,0,0)$处不连续，因而Gauss公式的区域中不能包含$(0,0,0)$。

取$S_2: x^2+y^2+z^2=\epsilon^2$外侧为正，则
$$
\begin{aligned}
\iint_{S_2} Pdydz+Qdzdx+Rdxdy
=&\iint_{S_2}\frac{xdydz+ydzdx+zdxdy}{\epsilon^3} \\
=&\frac1{\epsilon^3}\iiint_{V_2} 3 dV
=4\pi
\end{aligned}
$$
取$S_1: z=2, x^2+y^2\leq 4\times\frac89$上侧为正。
在曲面$S+S_1-S_2$中使用Gauss公式，有
$$
\iint_{S+S_1-S_2} Pdydz+Qdzdx+Rdxdy = 0
$$
从而
$$
\begin{aligned}
 \iint_{S} Pdydz+Qdzdx+Rdxdy
=&-\iint_{S_1} Pdydz+Qdzdx+Rdxdy \\
 &+\iint_{S_2} Pdydz+Qdzdx+Rdxdy
\end{aligned}
$$

而，记$D=\{x^2+y^2\leq \frac{32}9\}$，则
$$
\begin{aligned}
\iint_{S_1} Pdydz+Qdzdx+Rdxdy
=&\iint_D \frac{2}{(x^2+y^2+2^2)^{\frac32}} dxdy \\
=& \int_0^{2\pi} d\theta \int_0^{\frac{4\sqrt2}3} \frac{2}{(r^2+4)^{\frac32}} r dr \\
=&2\pi \int_0^{\frac{4\sqrt 2}3}\frac1{(r^2+4)^{\frac32}} d (r^2) \\
=&2\pi (-2)\frac1{\sqrt{t+4}}\big|_{t=0}^{t=\frac{32}9}
=4\pi\left(\frac12-\frac1{2\sqrt{17}}\right)
\end{aligned}
$$
因此，积分值为
$$
4\pi\left(1-\frac12+\frac{3}{2\sqrt{17}}\right)
=2\pi\left(1+\frac{3}{\sqrt{17}}\right)
$$
</div>

