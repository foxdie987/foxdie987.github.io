---
title: themeinstall
date: 2021-11-15 11:18:17
permalink: /pages/adf905/
sidebar: auto
categories:
  - 随笔
tags:
  -
---
# Theme install

## Step 1

``` shell
npm install -D vuepress

npm install vuepress-theme-vdoing -D

npm run dev # or yarn dev

```

## Step 2

``` js
// config.js
module.exports = {
  theme: 'vdoing',
  themeConfig: {
     sidebar: 'structuring' //  'structuring' | { mode: 'structuring', collapsable: Boolean} | 'auto' | 自定义
  }
}
```
