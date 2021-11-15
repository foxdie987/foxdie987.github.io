---
prev: ./note1.md
next: false
title: note2
date: 2021-11-11 17:44:48
permalink: /pages/1105a1/
sidebar: auto
categories: 
  - 随笔
tags: 
  - 
---

# Note 2

GO TO [ [note1](./note1.md) ]

## WEBP

[https://developers.google.com/speed/webp](https://developers.google.com/speed/webp)

The bin/ directory contains tools for encoding (**cwebp.exe**) and
decoding (**dwebp.exe**) images.

The easiest use should look like:
``` shell
  cwebp input.png -q 80 -o output.webp
```
which will convert the input file to a WebP file using a quality factor of 80
on a 0->100 scale (0 being the lowest quality, 100 being the best. Default
value is 75).
You might want to try the -lossless flag too, which will compress the source
(in RGBA format) without any loss. The -q quality parameter will in this case
control the amount of processing time spent trying to make the output file as
small as possible.


## Markdown guide

Go to
- [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)

- [https://guides.github.com/features/mastering-markdown/](https://guides.github.com/features/mastering-markdown)

### Links:
- Text in [] and URL goes in ()
``` md
[text](URL)
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
```
Result: [Duck Duck Go](https://duckduckgo.com).

- Text in [] and URL goes in (), text in this case can't have blank space.
``` md
[cmder](https://pquan.info/cmder-thay-the-hieu-qua-cho-command-promp-tren-windows)
```
Result: [cmder](https://pquan.info/cmder-thay-the-hieu-qua-cho-command-promp-tren-windows)

- Reference-style Links: are a special kind of link that make URLs easier to display and read in Markdown, keep the text easy to read.
``` md
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles" (ref link)
```
the rendered output:
> In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.
[1]:<https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

(ref link doesn't work?)

[Align Image in Markdown](https://davidwells.io/snippets/how-to-align-images-in-markdown)

## Math and Formula

[https://imronuke.wordpress.com/2012/02/17/how-to-convert-equation-in-mathtype-to-latex/](https://imronuke.wordpress.com/2012/02/17/how-to-convert-equation-in-mathtype-to-latex)

[https://tex.stackexchange.com/questions/233963/convert-mathtype-and-ms-word-equations-equations-to-latex](https://tex.stackexchange.com/questions/233963/convert-mathtype-and-ms-word-equations-equations-to-latex)

~~[https://github.com/maginapp/vuepress-plugin-katex](https://github.com/maginapp/vuepress-plugin-katex)~~

``` js
plugins: {
        '@maginapp/katex': {
          delimiters: 'dollars'
        }
    },
```

```md

$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$

Euler's identity $e^{i\pi}+1=0$ is a beautiful formula in $\mathbb{R}^2$.

Supposing that $y >= 0$ and that $[\log x]$ represents the integer part of $\log x$, let:

$$\Phi (y) = \frac {1} {2 \pi i} \int_{2 - i \infty}^{2 + i \infty} \frac {y^{\omega} \mathrm{d} \omega} {\omega \left(1 + \frac {\omega} {(\log x)^{1.1}}\right)^{[ \log x ] + 1}}, x > 1$$

Obviously, when $0 <= y <= 1$, there is $\Phi(y) = 0$. For all $y >= 0$, $\Phi(y)$ is a non-decreasing function.

When $\log x>=10^4$ and $y>= e^{2{(\log x)}^{-0.1}}$, thus:

$$1 - x^{- 0.1} <= \Phi (y) <= 1$$

$$\Phi (y) = \frac {1} {2 \pi i}$$
```
```md
\(Gamma(n) = (n-1)!\quad\forall n\in\mathbb N\)

Euler's identity \(e^{i\pi}+1=0\) is a beautiful formula in \(\mathbb{R}^2\).

Supposing that \(y >= 0\) and that \([\log x]\) represents the integer part of $\log x\), let:

\[\Phi (y) = \frac {1} {2 \pi i} \int_{2 - i \infty}^{2 + i \infty} \frac {y^{\omega} \mathrm{d} \omega} {\omega \left(1 + \frac {\omega} {(\log x)^{1.1}}\right)^{[ \log x ] + 1}}, x > 1\]

Obviously, when \(0 <= y <= 1\), there is \(\Phi(y) = 0\). For all \(y >= 0\), \(\Phi(y)\) is a non-decreasing function.

When \(\log x>=10^4\) and \(y>= e^{2{(\log x)}^{-0.1}}\), thus:

\[1 - x^{- 0.1} <= \Phi (y) <= 1\]

```

$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$

Euler's identity $e^{i\pi}+1=0$ is a beautiful formula in $\mathbb{R}^2$.

Supposing that $y >= 0$ and that $[\log x]$ represents the integer part of $\log x$, let:

$$\Phi (y) = \frac {1} {2 \pi i} \int_{2 - i \infty}^{2 + i \infty} \frac {y^{\omega} \mathrm{d} \omega} {\omega \left(1 + \frac {\omega} {(\log x)^{1.1}}\right)^{[ \log x ] + 1}}, x > 1$$

Obviously, when $0 <= y <= 1$, there is $\Phi(y) = 0$. For all $y >= 0$, $\Phi(y)$ is a non-decreasing function.

When $\log x>=10^4$ and $y>= e^{2{(\log x)}^{-0.1}}$, thus:

$$1 - x^{- 0.1} <= \Phi (y) <= 1$$

~~Supported Functions: [https://katex.org](https://katex.org/docs/supported.html)~~

**Note:** There is **problem** with bracket { } when convert MathType form MS Word to LaTeX 2.09. If too many { } brackets than necessary, **npm run build** will fail with errors.
Since KaTeX seems to require less { } in formula. Solution is that manually deleting redundant { } brackets after conversion will work, but if there are so many math formula in document
then it'll become a boring chore. => need a more refined answer to this hurdle (some tool maybe, or a fine LaTeX/MathJax plugin).

<mark style="background-color: Gold">As for now</mark>, since I has some problem with KaTeX plugin (can't make it work anymore), switch back to **MathJax**:
=> It also allows quickly copy converted MathType formula to .md file without editing { }.

[https://vuepress-community.netlify.app/en/plugins/mathjax/](https://vuepress-community.netlify.app/en/plugins/mathjax/)

``` js
plugins: [
[
  'vuepress-plugin-mathjax',
  {
    target: 'svg',
    macros: {
      '*': '\\times',
    },
  },
], ['aplayer']],
}
```
## Photoshop and Krita

I'm using [Krita](https://krita.org/en/) as a light weight Image Editor, portable-app ready. I'm still using Photoshop but if my machine I'm working on doesn't have it installed, then I should just grab a portable Krita for a quick edit.

BTW, if you are a Photoshop user (like me) and you're looking for Eraser, then [check the doc](https://docs.krita.org/en/user_manual/introduction_from_other_software/introduction_from_photoshop.html?highlight=eraser).

## SSH

As SSH is built in with [Cmder](https://pquan.info/cmder-thay-the-hieu-qua-cho-command-promp-tren-windows/), you may use it anytime by typing: `ssh @ip [-p port]`

Here is an example: `ssh user@10.0.0.8 -p8888`

``` shell
ssh user@10.0.0.8 -p8888
```

## Youtube

[Under Tides BGM](https://www.youtube.com/watch?v=QR7vqVo0Ky4)


## Unsorted lists:

`Down here is my unsorted lists for anything catching my eyes:` (will be sorted into proper categories eventually)

Thank [Suisei Archive Guide](https://guide.suisei.cc) for bringing me the joyful adventure of Vue.Js and VuePress -> I have started creating this blog not so long after I visited that site and love it. :heart: Although I'm not even interested in [Hololive](https://virtualyoutuber.fandom.com/wiki/Hololive) :joy:

https://www.bookstack.cn/read/vuepress2-en/41c7610565ee1a40.md

https://www.reddit.com/r/vuejs/comments/qge221/what_backend_to_use_for_vue/

https://dev.to/frontendfoxes/build-a-beautiful-website-with-vuepress-and-tailwindcss--3a03

[https://github.com/HEIGE-PCloud/DoIt](https://github.com/HEIGE-PCloud/DoIt)

https://aozaki.cc

Python Tutorial: Web Scraping with Requests-HTML:
https://www.youtube.com/watch?v=a6fIbtFB46g

Python Tutorial: Web Scraping with BeautifulSoup and Requests:
https://www.youtube.com/watch?v=ng2o98k983k

Vue JS Crash Course 2021
https://www.youtube.com/watch?v=qZXt1Aom3Cs

https://code.visualstudio.com/docs/python/tutorial-django

:notes: [monster-siren.hypergryph.com/music](https://monster-siren.hypergryph.com/music#album) :notes:

[https://mrfz.fandom.com/wiki/Requiem#Romanized](https://mrfz.fandom.com/wiki/Requiem#Romanized) :musical_note:

[Bridge Technology Series: Improving Inspection Access at Segmental Bridge Abutments](https://youtu.be/ruldJ3zFeG8?list=PL5_sm9g9d4T3ymcxjfVEdYnd2-Hj-Fozl)

[https://www.udemy.com/course/practical-regex/](https://www.udemy.com/course/practical-regex/)

[https://web.archive.org/save](https://web.archive.org/save) => save an archive of webpage, just in case it's 404 in the future.

https://www.researchgate.net/figure/Hognestad-Parabola-30_fig10_40540797

[https://gofile.io/welcome](https://gofile.io/welcome)

[Zalgo Text](https://lingojam.com/ZalgoText)
