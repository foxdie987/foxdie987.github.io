---
prev: false
next: ./note2.md
title: note1
date: 2021-11-11 17:44:48
permalink: /pages/c8cd74/
sidebar: auto
categories: 
  - 随笔
tags: 
  - 
---


# Note 1

## For starters

[https://nodejs.org/en/docs](https://nodejs.org/en/docs)

[https://nodejs.org/en/docs/guides/getting-started-guide](https://nodejs.org/en/docs/guides/getting-started-guide)

Install tools and configuration manually: (after install NodeJs)

[https://github.com/nodejs/node-gyp#on-windows](https://github.com/nodejs/node-gyp#on-windows)

[https://topdev.vn/blog/npm-la-gi/">https://topdev.vn/blog/npm-la-gi/](https://topdev.vn/blog/npm-la-gi/">https://topdev.vn/blog/npm-la-gi/)

[https://hexo.io/themes](https://hexo.io/themes)

``` shell
found 0 vulnerabilities
npm notice
npm notice New patch version of npm available! 8.1.0 -> 8.1.1
npm notice Changelog: https://github.com/npm/cli/releases/tag/v8.1.1
npm notice Run npm install -g npm@8.1.1 to update!
npm notice
```

``` shell
wait Extracting site metadata...
tip Apply theme @vuepress/theme-default ...
tip Apply plugin container (i.e. "vuepress-plugin-container") ...
tip Apply plugin @vuepress/register-components (i.e. "@vuepress/plugin-register-components") ...
tip Apply plugin @vuepress/active-header-links (i.e. "@vuepress/plugin-active-header-links") ...
tip Apply plugin @vuepress/search (i.e. "@vuepress/plugin-search") ...
tip Apply plugin @vuepress/nprogress (i.e. "@vuepress/plugin-nprogress") ...

√ Client
  Compiled successfully in 15.75s

√ Server
  Compiled successfully in 8.93s

wait Rendering static HTML...
success Generated static files in docs.
```

``` shell
cd C:\VuePress
git init
git add -A
git commit -m 'deploy'
```

## VuePress Resources:

A curated list of awesome things related to VuePress:
[https://github.com/vuepress/awesome-vuepress](https://github.com/vuepress/awesome-vuepress)

[https://github.com/vuepress/awesome-vuepress#themes](https://github.com/vuepress/awesome-vuepress#themes)

[https://vuepress.vuejs.org/guide/getting-started.html#prerequisites](https://vuepress.vuejs.org/guide/getting-started.html#prerequisites)

[https://ehkoo.com/bai-viet/static-web-vuepress-github-pages](https://ehkoo.com/bai-viet/static-web-vuepress-github-pages)

[https://blog.howar31.com/vuepress-blog-tutorial/#so-why-vuepress-and-gitlab-pages](https://blog.howar31.com/vuepress-blog-tutorial/#so-why-vuepress-and-gitlab-pages)

You can use this component in a header to add some status for an API:
``` md
### Badge <Badge text="beta" type="warning"/> <Badge text="default theme"/>
```
<span style="color: blue">type</span> - string, optional value: "tip"|"warning"|"error", defaults to "tip".

color name's cheat sheet: [https://htmlcolorcodes.com/color-names/](https://htmlcolorcodes.com/color-names)

### Add Logo to nav bar:
[https://vuepress.vuejs.org/theme/default-theme-config.html#navbar-logo](https://vuepress.vuejs.org/theme/default-theme-config.html#navbar-logo)

### MathJax support:

[https://vuepress-community.netlify.app/en/plugins/mathjax/#installation](https://vuepress-community.netlify.app)

### Prev/Next Links:
You can also explicitly overwrite or disable them for individual pages with YAML front matter:
``` yaml
---
prev: ./some-other-page
next: false
---
```
### APlayer:

``` js
plugins: [
          '@maginapp/vuepress-plugin-katex', {
            delimiters: 'brackets'
          },
          'aplayer'  // npm install -D vuepress-plugin-aplayer
        ],
```
### External js Code

https://coderedirect.com/questions/53896/how-to-add-external-js-scripts-to-vuejs-components

https://titanwolf.org/Network/Articles/Article?AID=1fa12010-da8c-4df5-86af-19ab0bbcb3df

https://stackoverflow.com/questions/52836660/how-to-add-jquery-into-a-vuepress-file  <===

https://github.com/vuejs/vuepress/issues/790

## VuePress Themes:

- vuepress-theme-hope: like default theme, but much more built-in feature: [https://vuepress-theme-hope.github.io/FAQ/](https://vuepress-theme-hope.github.io/FAQ/)
- A simple and efficient VuePress knowledge management: [https://github.com/xugaoyi/vuepress-theme-vdoing](https://github.com/xugaoyi/vuepress-theme-vdoing)
- A nice vuepress blog theme: [https://github.com/yuicer/vuepress-theme-yuicer](https://github.com/yuicer/vuepress-theme-yuicer)

## VuePress Video:

Video display example:

<video width="620" height="300" controls>
  <source src="https://sample-videos.com/video123/mp4/480/big_buck_bunny_480p_1mb.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

``` html
<video width="560" height="240" controls>
  <source src="https://sample-videos.com/video123/mp4/480/big_buck_bunny_480p_1mb.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```

WebM format:

<video width="784" height="476" controls>
  <source src="https://files.catbox.moe/rrwfqg.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

``` html
<video width="804" height="496" controls>
  <source src="https://files.abc.xyz/video.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
```


## Issues:

- https://github.com/vuejs/vuepress/issues/1935

See: [https://vuepress.vuejs.org/guide/deploy.html#github-pages](https://vuepress.vuejs.org/guide/deploy.html#github-pages)

For example, I use base: <mark style="background-color: Gold">"/course-material/"</mark> <Badge text="ok"/>, and that works for me.

=> not neccessary anymore if you custom domain like [https://vue.pquan.info](https://vue.pquan.info)

- Weird encounter but *solved by change the name of post's picture folder* by something shorter and **is not same name** as post's name, log provided for future reference:

``` md
(undefined) ./abcd/xyz.md?vue&type=template&id=37f20fd6& (./node_modules/cache-loader/dist/cjs.js?{"cacheDirectory":"node_modules/@vuepress/core/node_modules/.cache/vuepress","cacheIdentifier":"4b61893c-vue-loader-template"}!./node_modules/vue-loader/lib/loaders/templateLoader.js??vue-loader-options!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??ref--1-1!./node_modules/@vuepress/markdown-loader??ref--1-2!./draft/concrete1.md?vue&type=template&id=37f20fd6&)
03:29:16.854	Module not found: Error: Can't resolve /abcd/xyz.
```

### CNAME

And furthermore, about CNAME and DNS:
[https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/troubleshooting-custom-domains-and-github-pages#cname-errors](CNAME error)

also, every <mark style="background-color: Green">vuepress build</mark> destroys CNAME in docs folder.

[https://stackoverflow.com/questions/58287673/vuepress-build-deletes-cname-file-in-docs-needed-for-github-pages-custom-domain](Possible fix?)

### Hero Image

The Hero image must go in the public directory (for default theme)

The default theme looks for its hero image not in the <mark style="background-color: Gold">/assets/img</mark> directory but in the <mark style="background-color: Green">/.vuepress/public</mark> directory.

Add the YAML line heroImage: /banner.png. The default theme looks for its hero image the public directory, which is found in /.vuepress/public.
The next thing to add is the directive heroText: ...

GO TO: [ [note2](./note2.md) ]
