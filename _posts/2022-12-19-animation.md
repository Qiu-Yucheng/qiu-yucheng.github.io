---
layout: post
title: 关于如何生成轻小说立绘
subtitle: 怄火
tags: 杂项
show: true
---

有四版，按时间倒序放在这里。

没有放的图，可以去/img/animation下面找。

-----

maple dream的背景

![img](/img/2023-02-24-maple-dream/bg.png)

这是我在为oωo那篇生成背景图的过程中随出来的。感觉很好看所以拿来用了。

img2img。seed在旁边放着。

promot: (masterpiece) (highres:1.3) (extremely detailed:1.2), (windy:1.1), (autumn:1.5) (maple tree graden:1.3), (high saturation:1.3), (high contrast:1.3), (bench:1.5), (2 girls on the bench:1.8) (facing each other:1.5), (flat chest), (jk uniform:1.5), (girlA sitting on the bench and brown hair and blue eyes:1.4) (and staring and tear stains:1.5) (and facing right:1.3), (girlB kneeling on the bench and black eyes and black hair and facing left and smiling:1.4) (and cupping and holding girlA's face:1.6), (side face:1.5), (✋:1.3), (extremely cute:1.5), (extremely detailed cute aqua eyes:1.5)

Negative prompt: (mutated hands and fingers:1.5 ), (long body :1.3), (mutation, poorly drawn :1.2), bad anatomy, liquid body, disfigured, malformed, mutated, anatomical nonsense, error, malformed hands, long neck, blurred, lowers, lowres, bad anatomy, bad proportions, bad shadow, uncoordinated body, unnatural body, bad hands, fused hand, missing hand, disappearing legs, text, ui, error, missing fingers, fused fingers, poorly drawn hands, more than 1 left hand, more than 1 right hand

Steps: 15, Sampler: Euler, CFG scale: 4, Seed: 4182836341, Size: 1280x768, Model hash: a3648a3cee, Denoising strength: 0.95, Mask blur: 0

promot其实是之前乱写的，换了目标之后有地方没有修捏。

然后我就大笔一挥题个题目。这就是bg.png.kra所做的。你可以用krita打开它。

-----

version 5

todo : 生成一张百合图。

关于stable diffusion。我的gpu是rtx3050，显存只有可怜的4g。开启--xformers --medvram --no-half-vae，可以在1280*768下得到3s/it的速度。不加最后一项我这里会玄学爆炸。

如果你的显存像我一样可怜，当你要生成一个可以不是非常细节的图的时候，不要开启--precision full或者--no-half，这会让你的显存需求翻倍，就不得不开--lowvram啦，而--lowvram用过的都知道它是下下策。当你要对着一张图精修的时候，可以尝试--precision full --no-half --lowvram能不能得到更好的效果。

-----

version 4

在version 3之上用sd img2img了一下。model是hiten-anything[9b4893ed]。

下面是陈老师。

![c.png](/img/animation/ver4/c.png)

下面是邱老师。

![q.png](/img/animation/ver4/q.png)

都非常帅呢。陈老师在选的时候实际上有五个候选，我们犹豫了一下然后我钦点了这个，并手动修了手部。不会简笔画。感觉衣服画的比较神。下面是另外四个陈老师，没有修手。

![ct1.png](/img/animation/ver4/ct1.png)

![ct2.png](/img/animation/ver4/ct2.png)

![ct3.png](/img/animation/ver4/ct3.png)

![ct4.png](/img/animation/ver4/ct4.png)

讲个笑话，当我想画一个弯曲的看起来像是小括号转过来的眉毛的时候，它给我来了这么一手。

![eat.png](/img/animation/ver4/eat.png)

不过这个的真实原因是我把round face的权重搞的太高了导致炸了。

-----

version 3

使用waifulabs生成了面部(并自己修了细节)，然后用stable diffusion生成了剩下的部分，使用的model是anything v3。

![D.png](/img/animation/ver3/D.png)

左边是陈语秋而右边是邱雨橙。感觉陈老师好帅而邱老师好可爱，看起来就是想要达成这样的目的呢。有时候我尝试穿的像陈老师一样帅，但是还是没有这个水平。突然想到是不是可以说披风/风衣是男人的裙子。

相比之下crypko就拉多了。不过好像他们那个生成上半身的技术还挺牛逼的。杂交啥的玩不懂。不过crypko的好处是给你修补的机会，waifulabs只能手动修。也好像以前是可以手写一个client来修的，现在不清楚了。sd画的太慢了，随一张好看的显卡得烧一年。

-----

version 2

很年轻的时候拿waifulabs跑的，然后ps把背景删了。

我认为邱老师是waifulabs生成过最成功的作品之一。陈老师是技术限制，当时第三版已经生成出来了，但是找不到合适的背景。

-----

version 1

更年轻的时候拿waifulabs跑的。那时候感觉我的风格跟现在可能不太一样呢。