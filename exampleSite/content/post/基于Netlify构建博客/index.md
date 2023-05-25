+++
author = "Rico0807"
title = "基于Netlify构建博客"
date = "2023-05-25"
description = "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags = [
    "markdown",
    "css",
    "html",
    "themes",
]
categories = [
    "themes",
    "syntax",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
image = "pawel-czerwinski-8uZPynIu-rQ-unsplash.jpg"
+++

## 基于Netlify构建博客

> 雨果官网：https://themes.gohugo.io/
>
> Netlify官网：https://app.netlify.com/
>
> Git官网：https://git-scm.com/



## 基于Git更新GitHub库

基本步骤：

> Step_01：在根目录下打开 Git Bash
>
> Step_02：将GitHub库中的工程文件下载至根目录
>
> Step_03：在下载好的文件中对源码进行修改
>
> Step_04：上传

```git
git clone [url]

git add *
git commit -m "change"
git push [url] master
```

【注】：

> 1.在执行`git commit -m "change"`报错时，一般是 user.name 和 user.email未定义，通常使用`git config --global user.name xxxx`和`git config --global user.email xxxx`进行定义。
>
> 2.在第一次执行`git push [url] master`后会出现GitHub的授权或登录界面，按要求授权或登录即可完成更新上传。
